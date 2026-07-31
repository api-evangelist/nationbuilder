---
name: Run a petition and collect signatures
description: Create a petition and add/list supporter signatures in NationBuilder v2.
api: openapi/nationbuilder-v2-openapi-original.yml
operations: [createPetition, listPetitions, showPetition, createPetitionSignature, listPetitionSignatures]
generated: '2026-07-20'
method: generated
source: openapi/nationbuilder-v2-openapi-original.yml
---

# Run a petition and collect signatures

## Preconditions
- OAuth 2.0 bearer token; `application/vnd.api+json`; nation-scoped host.

## Steps
1. **Create the petition** — `createPetition` (JSON:API `data`, `type: "petitions"`); capture the petition `id`. Or `listPetitions` / `showPetition` to reuse an existing one.
2. **Record a signature** — `createPetitionSignature` with `relationships.petition` and `relationships.signup` linkages (a signature `belongs_to` both a petition and a signup). Returns `201`.
3. **Report** — `listPetitionSignatures` filtered to the petition to tally signatures; page with `page[size]` / `page[number]`.

## Rules
- A petition signature requires both the petition `id` and a signup `id` (create the signup first if needed via `createSignup`).
- `422` for validation errors (JSON:API `errors[]`); `429` rate-limited — honor `Retry-After`.
