---
name: Create an event and manage RSVPs
description: Create an event and record/list attendee RSVPs in NationBuilder v2.
api: openapi/nationbuilder-v2-openapi-original.yml
operations: [createEvent, listEvents, showEvent, createEventRsvp, listEventRsvps]
generated: '2026-07-20'
method: generated
source: openapi/nationbuilder-v2-openapi-original.yml
---

# Create an event and manage RSVPs

## Preconditions
- OAuth 2.0 bearer token; `application/vnd.api+json`; nation-scoped host.

## Steps
1. **Create the event** — `createEvent` (JSON:API `data`, `type: "events"`); capture the event `id`. Or discover with `listEvents` / `showEvent`.
2. **Record an RSVP** — `createEventRsvp` linking the event and the attendee signup (create the signup first with `createSignup` if the attendee is new). Returns `201`.
3. **List attendees** — `listEventRsvps` filtered to the event; page with `page[size]` / `page[number]`.

## Rules
- An RSVP links an event and a signup — set both relationship linkages.
- Handle `422` validation errors and `429` rate limits (`Retry-After`).
