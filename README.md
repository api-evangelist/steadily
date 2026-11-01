# Steadily

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

Steadily is a US landlord-insurance provider — built by landlords, for landlords — writing rental-property policies in all 50 states with online quotes in minutes and coverage designed around how rental properties actually work. Its Partner API, a FastAPI-based REST service at api.steadily.com, lets property managers, lenders, and marketplaces generate instant insurance estimates, refer leads, and track bound policies. Appointed independent agencies use the companion Rater Quotes API to create, price, underwrite, and offer quotes directly from their rater. Steadily was founded by a landlord who could not find decent insurance for his own rental property.

**Areas:** Company · Fintech · Insurance · Landlord Insurance · Insurtech · Real Estate · Rental Property

## Steadily on APIs.io

Everything profiled for Steadily is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/steadily/](https://apis.io/providers/steadily/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [Steadily Account API](https://apis.io/apis/steadily/steadily-account-api/) — Steadily uses Bearer Tokens to authenticate requests to the quoting endpoints on behalf of some appointed agent. There's two steps to this process: 1. Use…
- [Steadily Draft Quote API](https://apis.io/apis/steadily/steadily-draft-quote-api/) — A Draft Quote is an editable draft of a policy. Create a new draft quote by passing in basic insured and property information to `POST…
- [Steadily Lead Referrals API](https://apis.io/apis/steadily/steadily-lead-referrals-api/) — Submit and retrieve lead referrals. Use the refer lead endpoint to submit a lead with full quote details and start the insurance quote process. You'll get…
- [Steadily Lender API](https://apis.io/apis/steadily/steadily-lender-api/) — Policy information and change requests for third-party lender integrations
- [Steadily Policy API](https://apis.io/apis/steadily/steadily-policy-api/) — A Policy is an issued insurance policy. The declaration document and policy packet are available.
- [Steadily Quote Estimates API](https://apis.io/apis/steadily/steadily-quote-estimates-api/) — The Instant Estimate API is a one-step express API to quickly get a landlord insurance estimate you can display within your platform. To get started, you…
- [Steadily Quote Offer API](https://apis.io/apis/steadily/steadily-quote-offer-api/) — An Offer is an immutable offer for coverage extended to a customer. Offers are generated from draft quotes and provides a PDF quote document. Creating an…
- [Steadily Reporting API](https://apis.io/apis/steadily/steadily-reporting-api/) — Reporting on the referrals you've sent Steadily and the referral fees you've earned. The lead, account, and policy endpoints follow each referral through…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [steadily-partner](https://apis.io/servers/steadily/steadily-partner/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Steadily Agentic Access](https://apis.io/agentic-access/steadily/steadily-agentic-access/)

#### Collections (8)

Postman and Open Collection request collections.

- [Partner Account API](https://apis.io/collections/steadily/open-steadily-account-api/)
- [Partner Account Draft Quote API](https://apis.io/collections/steadily/open-steadily-draft-quote-api/)
- [Partner Account Lead Referrals API](https://apis.io/collections/steadily/open-steadily-lead-referrals-api/)
- [Partner Account Lender API](https://apis.io/collections/steadily/open-steadily-lender-api/)
- [Partner Account Policy API](https://apis.io/collections/steadily/open-steadily-policy-api/)
- [Partner Account Quote Estimates API](https://apis.io/collections/steadily/open-steadily-quote-estimates-api/)
- [Partner Account Quote Offer API](https://apis.io/collections/steadily/open-steadily-quote-offer-api/)
- [Partner Account Reporting API](https://apis.io/collections/steadily/open-steadily-reporting-api/)

#### Overlays (3)

OpenAPI overlays, including conversational phrasing for each operation.

- [Steadily Estimate Api Overlay](https://apis.io/overlays/steadily/steadily-estimate-api-overlay/)
- [Steadily Partner Overlay](https://apis.io/overlays/steadily/steadily-partner-overlay/)
- [Steadily Rater Quotes Overlay](https://apis.io/overlays/steadily/steadily-rater-quotes-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Steadily Authentication](https://apis.io/security/steadily/steadily-authentication/)
- [Steadily Domain Security](https://apis.io/security/steadily/steadily-domain-security/)
- [Steadily Vulnerability Disclosure](https://apis.io/security/steadily/steadily-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://steadily.com)
- [Documentation](https://api.steadily.com/redoc)
- [Getting started](https://www.steadily.com/api)
- [API reference](https://api.steadily.com/estimate-api/redoc)
- [Sign up](https://www.steadily.com/partners)
- [Blog](https://www.steadily.com/blog)
- [Security](https://www.steadily.com/security)
- [Privacy policy](https://www.steadily.com/privacy-policy)

## API Evangelist rating

**Kin Score 35.4** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 42.7 |
| Contract governance | 4.5 |
| Operational transparency | 10.5 |
| Developer ergonomics | 49.4 |
| Access clarity | 23.7 |

**Agent readiness 23.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
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

**Regulatory alignment 23.7** — Insurance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/steadily/](https://apis.io/providers/steadily/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Steadily: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/steadily/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
