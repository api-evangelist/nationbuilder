---
name: Sync a supporter into a NationBuilder nation
description: Find or create a person (signup) in a nation and apply a tag, using the JSON:API v2 API.
api: openapi/nationbuilder-v2-openapi-original.yml
operations: [listSignups, createSignup, showSignup, updateSignup, createSignupTag, createSignupTagging]
generated: '2026-07-20'
method: generated
source: openapi/nationbuilder-v2-openapi-original.yml
---

# Sync a supporter into a NationBuilder nation

Use the NationBuilder V2 API (JSON:API) to upsert a supporter record and tag them.

## Preconditions
- OAuth 2.0 bearer token for the target nation (`Authorization: Bearer <token>`).
- Base host is nation-scoped: `https://{nation-slug}.nationbuilder.com`.
- Send and accept `application/vnd.api+json`. Bodies use the JSON:API `data` envelope (`type: "signups"`, `attributes: {...}`).

## Steps
1. **Look for an existing person** — `listSignups` with a `filter` on email so you do not create a duplicate. Index endpoints return 20 per page; page with `page[size]` / `page[number]`.
2. **Create if absent** — `createSignup` with the person's attributes (email, first_name, last_name). On success you get `201` and the new resource `id`.
3. **Otherwise update** — `updateSignup` (PATCH) with the resource `id` to fill in changed attributes.
4. **Ensure the tag exists** — `createSignupTag` (idempotent by name; ignore the conflict if it already exists).
5. **Apply the tag** — `createSignupTagging` linking the signup `id` to the tag.
6. **Confirm** — `showSignup` with `include` to sideload the taggings and verify.

## Rules
- No request-level idempotency key is offered; guard creates with the `listSignups` lookup in step 1 to avoid duplicates.
- On `429`, honor `Retry-After` (limit is ~250 requests / 10s per token and per IP).
- Validation failures return `422` with a JSON:API `errors[]` array — read `errors[].detail` / `errors[].source`.
