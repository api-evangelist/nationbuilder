# NationBuilder

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

NationBuilder is a community-engagement and organizing platform for political campaigns, advocacy groups, nonprofits, and membership organizations, pairing a supporter CRM with a website/page builder, email and text messaging, event and petition tools, and integrated fundraising. Its developer surface is a REST API offered in two flavors: the current v2 API, which follows the JSON:API specification and authenticates with OAuth 2.0 (authorization-code with optional PKCE and refresh tokens), and a legacy v1 API that uses per-nation API tokens. The API exposes people/signups, donations, events, petitions, memberships, lists, tags, and related resources so integrators can sync supporter data and automate outreach. NationBuilder is multi-tenant: each nation is reached at its own {nation-slug}.nationbuilder.com host.

**Areas:** Community Organizing · CRM · Political · Non-Profit · Fundraising · Advocacy · Website Builder · Event · Email · JSON:API

## NationBuilder on APIs.io

Everything profiled for NationBuilder is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nationbuilder/](https://apis.io/providers/nationbuilder/)** — or go straight to one of the APIs or properties below.

### APIs (41)

- [NationBuilder Async Processes API](https://apis.io/apis/nationbuilder/nationbuilder-async-processes-api/) — This endpoint is used to get information about deferred or asynchronous processes returned by other endpoints such as adding and removing signups from a…
- [NationBuilder Automation Enrollments API](https://apis.io/apis/nationbuilder/nationbuilder-automation-enrollments-api/) — AutomationEnrollments link signups to automations. Every AutomationEnrollment belongs to a single Signup and a single Automation. Further information on how…
- [NationBuilder Automations API](https://apis.io/apis/nationbuilder/nationbuilder-automations-api/) — Automations represent workflows where chains of actions and reactions can be created within a nation. Signups can be enrolled in an automation and are…
- [NationBuilder Ballots API](https://apis.io/apis/nationbuilder/nationbuilder-ballots-api/) — Ballots are a record of an election and how a person voted for said election. Each ballot is associated with a voter and an election and contains…
- [NationBuilder Broadcasters API](https://apis.io/apis/nationbuilder/nationbuilder-broadcasters-api/) — Broadcasters are the voices who speak publicly on behalf of your nation. All external communications are organized around broadcasters.
- [NationBuilder Contacts API](https://apis.io/apis/nationbuilder/nationbuilder-contacts-api/) — Contacts are logged interactions between people in your nation. More information about contacts and the fields found in the UI and API interfaces can be…
- [NationBuilder Custom Fields API](https://apis.io/apis/nationbuilder/nationbuilder-custom-fields-api/) — Custom fields are available for Signups and Donations. See [here](https://support.nationbuilder.com/en/articles/2340612-introduction-to-custom-fields) for…
- [NationBuilder Donation Tracking Codes API](https://apis.io/apis/nationbuilder/nationbuilder-donation-tracking-codes-api/) — Tracking codes are used to identify where a financial transaction came from. Users give the tracking code a custom name/slug and use the code to track where…
- [NationBuilder Donations API](https://apis.io/apis/nationbuilder/nationbuilder-donations-api/) — Currently we allow you to record existing donation transactions via API V2. These transactions will not be backed by any kind of financial transaction. See…
- [NationBuilder Elections API](https://apis.io/apis/nationbuilder/nationbuilder-elections-api/) — Elections are available on nations with voter features enabled. See more information about election functionality…
- [NationBuilder Event Rsvps API](https://apis.io/apis/nationbuilder/nationbuilder-event-rsvps-api/) — This resource is for creating, reading, updating, and deleting Event RSVPs. When creating event RSVPs, the rsvp must be given signup data, either by passing…
- [NationBuilder Event Ticket Levels API](https://apis.io/apis/nationbuilder/nationbuilder-event-ticket-levels-api/) — This resource is for creating, reading, updating, and deleting ticket levels for events. manage the ticket levels available for the events. Ticket levels…
- [NationBuilder Events API](https://apis.io/apis/nationbuilder/nationbuilder-events-api/) — Resource used for managing event data associated with event pages. More details on events within NationBuilder can be found…
- [NationBuilder Imports API](https://apis.io/apis/nationbuilder/nationbuilder-imports-api/) — All kinds of data can be imported into a nation, when this happens we create an import resource as a record of the imported data. Each import has a type…
- [NationBuilder Lists API](https://apis.io/apis/nationbuilder/nationbuilder-lists-api/) — Lists are collections of signups. Often created from filters they are useful for grouping signups together by common attributes. They can be used to perform…
- [NationBuilder Mailings API](https://apis.io/apis/nationbuilder/nationbuilder-mailings-api/) — Referred to as email blasts, mailings send bulk emails to a group of signups at once. Mailings belong to and are sent via a broadcaster. The recipients of a…
- [NationBuilder Membership Types API](https://apis.io/apis/nationbuilder/nationbuilder-membership-types-api/) — Membership types are used to identify memberships assigned to signups. A membership type has many memberships which are assigned a single signup. The only…
- [NationBuilder Memberships API](https://apis.io/apis/nationbuilder/nationbuilder-memberships-api/) — A membership is a way to organize supporters and provide additional benefits based on actions they've taken or money donated. More information about…
- [NationBuilder Pages API](https://apis.io/apis/nationbuilder/nationbuilder-pages-api/) — Pages are published on your site. Each page type offers different features, you can view them…
- [NationBuilder Path Histories API](https://apis.io/apis/nationbuilder/nationbuilder-path-histories-api/) — Documents a signup's step along a path journey.
- [NationBuilder Path Journey Status Changes API](https://apis.io/apis/nationbuilder/nationbuilder-path-journey-status-changes-api/) — Documents the status change of a path journey.
- [NationBuilder Path Journeys API](https://apis.io/apis/nationbuilder/nationbuilder-path-journeys-api/) — Path journeys are the relationship between signups and paths. Further information available…
- [NationBuilder Path Steps API](https://apis.io/apis/nationbuilder/nationbuilder-path-steps-api/) — Path steps name the positions within a path a signup can be assigned to. Further information available…
- [NationBuilder Paths API](https://apis.io/apis/nationbuilder/nationbuilder-paths-api/) — Paths store information about path journeys and steps. They are related to signups via path journeys. A path can be assigned many path journeys and path…
- [NationBuilder Petition Signatures API](https://apis.io/apis/nationbuilder/nationbuilder-petition-signatures-api/) — Petition signatures are the relationship between petitions and signups.
- [NationBuilder Petitions API](https://apis.io/apis/nationbuilder/nationbuilder-petitions-api/) — Petitions are pages on your site that can be signed and shared by your supporters. Learn more about them…
- [NationBuilder Pledges API](https://apis.io/apis/nationbuilder/nationbuilder-pledges-api/) — Pledges are a promise from a signup to donate to your cause. These are not donations. Further information available…
- [NationBuilder Precincts API](https://apis.io/apis/nationbuilder/nationbuilder-precincts-api/) — Precincts are districts used by political campaigns. Read more about them…
- [NationBuilder Relationships API](https://apis.io/apis/nationbuilder/nationbuilder-relationships-api/) — Valid relationship types are ["affiliate-affiliate", "alum-school", "assistant-assisted", "board_member-organization", "candidate-committee",…
- [NationBuilder Signup Profiles API](https://apis.io/apis/nationbuilder/nationbuilder-signup-profiles-api/) — Profile information for a signup that can be displayed on a public site page. Read more on public profiles…
- [NationBuilder Signup Taggings API](https://apis.io/apis/nationbuilder/nationbuilder-signup-taggings-api/) — Signup taggings are the relation between a signup and a tag.
- [NationBuilder Signup Tags API](https://apis.io/apis/nationbuilder/nationbuilder-signup-tags-api/) — Tags are used to quickly identify signups by certain characteristics. They are related to signups through SignupTaggings. Read more about them…
- [NationBuilder Signups API](https://apis.io/apis/nationbuilder/nationbuilder-signups-api/) — Signups store information about people in your nation. Further information available…
- [NationBuilder Sites API](https://apis.io/apis/nationbuilder/nationbuilder-sites-api/) — A site is how supporters interact with your nation. Each site has a theme and many pages that can be drafted and published later to be viewed publicly. Read…
- [NationBuilder Suggestion Boxes API](https://apis.io/apis/nationbuilder/nationbuilder-suggestion-boxes-api/) — Suggestion boxes are containers for collecting suggestions from your community. They live on website pages, and define the settings, auto-responses,…
- [NationBuilder Suggestions API](https://apis.io/apis/nationbuilder/nationbuilder-suggestions-api/) — Suggestions are individual ideas or proposals submitted to suggestion boxes on your site. They can be responded to, categorized, and managed by…
- [NationBuilder Survey Question Possible Responses API](https://apis.io/apis/nationbuilder/nationbuilder-survey-question-possible-responses-api/) — The potential answers to a survey question.
- [NationBuilder Survey Question Responses API](https://apis.io/apis/nationbuilder/nationbuilder-survey-question-responses-api/) — User responses to Survey Questions.
- [NationBuilder Survey Questions API](https://apis.io/apis/nationbuilder/nationbuilder-survey-questions-api/) — Questions asked within a survey.
- [NationBuilder Surveys API](https://apis.io/apis/nationbuilder/nationbuilder-surveys-api/) — Surveys have questions with possible responses. These questions also have responses from the users.
- [NationBuilder Voters API](https://apis.io/apis/nationbuilder/nationbuilder-voters-api/) — Voter records store the ballot history of a single signup.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [nationbuilder](https://apis.io/servers/nationbuilder/nationbuilder/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Nationbuilder Agentic Access](https://apis.io/agentic-access/nationbuilder/nationbuilder-agentic-access/)

#### Collections (41)

Postman and Open Collection request collections.

- [NationBuilder V2 Async Processes API](https://apis.io/collections/nationbuilder/open-nationbuilder-async-processes-api/)
- [NationBuilder V2 Async Processes Automation Enrollments API](https://apis.io/collections/nationbuilder/open-nationbuilder-automation-enrollments-api/)
- [NationBuilder V2 Async Processes Automations API](https://apis.io/collections/nationbuilder/open-nationbuilder-automations-api/)
- [NationBuilder V2 Async Processes Ballots API](https://apis.io/collections/nationbuilder/open-nationbuilder-ballots-api/)
- [NationBuilder V2 Async Processes Broadcasters API](https://apis.io/collections/nationbuilder/open-nationbuilder-broadcasters-api/)
- [NationBuilder V2 Async Processes Contacts API](https://apis.io/collections/nationbuilder/open-nationbuilder-contacts-api/)
- [NationBuilder V2 Async Processes Custom Fields API](https://apis.io/collections/nationbuilder/open-nationbuilder-custom-fields-api/)
- [NationBuilder V2 Async Processes Donation Tracking Codes API](https://apis.io/collections/nationbuilder/open-nationbuilder-donation-tracking-codes-api/)
- [NationBuilder V2 Async Processes Donations API](https://apis.io/collections/nationbuilder/open-nationbuilder-donations-api/)
- [NationBuilder V2 Async Processes Elections API](https://apis.io/collections/nationbuilder/open-nationbuilder-elections-api/)
- [NationBuilder V2 Async Processes Event Rsvps API](https://apis.io/collections/nationbuilder/open-nationbuilder-event-rsvps-api/)
- [NationBuilder V2 Async Processes Event Ticket Levels API](https://apis.io/collections/nationbuilder/open-nationbuilder-event-ticket-levels-api/)
- [NationBuilder V2 Async Processes Events API](https://apis.io/collections/nationbuilder/open-nationbuilder-events-api/)
- [NationBuilder V2 Async Processes Imports API](https://apis.io/collections/nationbuilder/open-nationbuilder-imports-api/)
- [NationBuilder V2 Async Processes Lists API](https://apis.io/collections/nationbuilder/open-nationbuilder-lists-api/)
- [NationBuilder V2 Async Processes Mailings API](https://apis.io/collections/nationbuilder/open-nationbuilder-mailings-api/)
- [NationBuilder V2 Async Processes Membership Types API](https://apis.io/collections/nationbuilder/open-nationbuilder-membership-types-api/)
- [NationBuilder V2 Async Processes Memberships API](https://apis.io/collections/nationbuilder/open-nationbuilder-memberships-api/)
- [NationBuilder V2 Async Processes Pages API](https://apis.io/collections/nationbuilder/open-nationbuilder-pages-api/)
- [NationBuilder V2 Async Processes Path Histories API](https://apis.io/collections/nationbuilder/open-nationbuilder-path-histories-api/)
- [NationBuilder V2 Async Processes Path Journey Status Changes API](https://apis.io/collections/nationbuilder/open-nationbuilder-path-journey-status-changes-api/)
- [NationBuilder V2 Async Processes Path Journeys API](https://apis.io/collections/nationbuilder/open-nationbuilder-path-journeys-api/)
- [NationBuilder V2 Async Processes Path Steps API](https://apis.io/collections/nationbuilder/open-nationbuilder-path-steps-api/)
- [NationBuilder V2 Async Processes Paths API](https://apis.io/collections/nationbuilder/open-nationbuilder-paths-api/)
- [NationBuilder V2 Async Processes Petition Signatures API](https://apis.io/collections/nationbuilder/open-nationbuilder-petition-signatures-api/)
- …and 16 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Nationbuilder V2 Overlay](https://apis.io/overlays/nationbuilder/nationbuilder-v2-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Nationbuilder Authentication](https://apis.io/security/nationbuilder/nationbuilder-authentication/)
- [Nationbuilder Domain Security](https://apis.io/security/nationbuilder/nationbuilder-domain-security/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Nationbuilder Plans Pricing](https://apis.io/plans/nationbuilder/nationbuilder-plans-pricing/)
- [Nationbuilder Price Estimates](https://apis.io/plans/nationbuilder/nationbuilder-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Nationbuilder Rate Limits](https://apis.io/rate-limits/nationbuilder/nationbuilder-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://nationbuilder.com)
- [Documentation](https://support.nationbuilder.com/en/collections/10408291-api)
- [Getting started](https://support.nationbuilder.com/en/articles/9869274-nationbuilder-api-quickstart-guide)
- [Pricing](https://nationbuilder.com/pricing)
- [Sign up](https://nationbuilder.com/signup)
- [Support](https://support.nationbuilder.com/)
- [Changelog](https://support.nationbuilder.com/en/articles/2869824-where-can-i-find-out-what-s-new-or-been-updated-fixed-in-nationbuilder)
- [Blog](https://nationbuilder.com/blog)
- [Terms of service](https://nationbuilder.com/tos)
- [Privacy policy](https://nationbuilder.com/privacy)
- [GitHub](https://github.com/nationbuilder)
- [Status](https://status.nationbuilder.com/)

## API Evangelist rating

**Kin Score 61.8** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 54.3 |
| Contract governance | 18.2 |
| Operational transparency | 63.2 |
| Developer ergonomics | 58.9 |
| Access clarity | 76.3 |

**Agent readiness 37.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | verified |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 24.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nationbuilder/](https://apis.io/providers/nationbuilder/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for NationBuilder: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nationbuilder/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
