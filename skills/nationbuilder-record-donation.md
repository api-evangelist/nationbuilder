---
name: Record a donation for a supporter
description: Create (or locate) a signup and record a donation against them in NationBuilder v2.
api: openapi/nationbuilder-v2-openapi-original.yml
operations: [listSignups, createSignup, createDonation, showDonation, listDonations]
generated: '2026-07-20'
method: generated
source: openapi/nationbuilder-v2-openapi-original.yml
---

# Record a donation for a supporter

## Preconditions
- OAuth 2.0 bearer token for the nation; `application/vnd.api+json` request/response.
- Nation-scoped host `https://{nation-slug}.nationbuilder.com`.

## Steps
1. **Resolve the donor** — `listSignups` filtered by email; if none, `createSignup` to get a signup `id`.
2. **Create the donation** — `createDonation` with a JSON:API `data` body (`type: "donations"`) carrying the amount and a `relationships.signup` linkage to the donor `id`. Success returns `201`.
3. **Verify** — `showDonation` with the returned `id`, or `listDonations` filtered to the donor to reconcile.

## Rules
- Donations belong to a signup (`belongs_to` via the `signup` relationship) — always set the linkage.
- No idempotency-key header exists; if you must avoid double-charging, check `listDonations` for a matching recent record before creating.
- Handle `422` (validation) and `429` (rate limit, honor `Retry-After`).
