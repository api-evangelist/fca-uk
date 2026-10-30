# Financial Conduct Authority

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

The Financial Conduct Authority (FCA) is the United Kingdom's conduct regulator for around 42,000 financial services firms and the prudential regulator for most non-bank firms, operating alongside the Prudential Regulation Authority under the dual-regulation model. In insurance the FCA owns conduct regulation of general insurance and protection markets through ICOBS and the Consumer Duty, authorises and supervises insurers, Lloyd's managing agents, MGAs, brokers and appointed representatives, and publishes market-wide insurance data such as the annual General Insurance Value Measures. Its API posture is that of a regulator, not a carrier: there is no open-insurance obligation in the UK and the FCA publishes no insurance product API of its own. It does operate two genuine public APIs. The Financial Services Register API at register.fca.org.uk/services/V0.1 exposes firm, individual and fund authorisation records including insurance permissions and appointed-representative relationships; access is free and self-serve but the developer portal and its reference documentation sit behind a Salesforce registration login, and authentication is by X-Auth-Email and X-Auth-Key headers. The data publication API at api.data.fca.org.uk is an anonymous OpenSearch-style query interface over FIRDS and FITRS file artefacts, documented in the FCA's own published technical specifications — markets reference data, not insurance data. Neither API has an OpenAPI definition. Everything else the FCA publishes for the insurance market is documents and spreadsheets: the Handbook, market bulletins, consultation papers, and XLSX data releases. The FCA's Open Finance roadmap of 14 April 2026 names insurance as an in-scope sector but remains a vision document, with a formal discussion paper on the first scheme not due until Q4 2026, so no insurance data-sharing API mandate exists. No ACORD reference appears anywhere on fca.org.uk.

**Areas:** Insurance · United Kingdom · Regulator · Market Infrastructure · Financial Services · Public Register · Conduct Regulation · Open Finance · Insurance Intermediaries · Risk Data · Market Data · Reference Data

## Financial Conduct Authority on APIs.io

Everything profiled for Financial Conduct Authority is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fca-uk/](https://apis.io/providers/fca-uk/)** — or go straight to one of the APIs or properties below.

### APIs (2)

- [FCA Financial Services Register API](https://apis.io/apis/fca-uk/fca-financial-services-register-api/) — Read-only REST API over the Financial Services Register, the FCA's public record of authorised firms, individuals, funds and appointed representatives.…
- [FCA Data Publication API (FIRDS / FITRS)](https://apis.io/apis/fca-uk/fca-data-publication-api/) — Anonymous machine-to-machine query interface over the file artefacts the FCA publishes through data.fca.org.uk, documented in the FCA's own FIRDS and FITRS…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Fca Uk Authentication](https://apis.io/security/fca-uk/fca-uk-authentication/)
- [Fca Uk Domain Security](https://apis.io/security/fca-uk/fca-uk-domain-security/)

#### Rate limits (1)

Published request limits.

- [Fca Uk Rate Limits](https://apis.io/rate-limits/fca-uk/fca-uk-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.fca.org.uk/)
- [Documentation](https://www.fca.org.uk/firms/financial-services-register)
- [API reference](https://register.fca.org.uk/Developer/s/)
- [Pricing](https://www.fca.org.uk/firms/financial-services-register/data-extract)
- [Sign up](https://register.fca.org.uk/Developer/ShAPI_LoginPage?ec=302&startURL=%2FDeveloper%2Fs%2F)
- [Support](https://www.fca.org.uk/contact)
- [Blog](https://www.fca.org.uk/news)
- [Terms of service](https://www.fca.org.uk/legal)
- [Privacy policy](https://www.fca.org.uk/privacy)

## API Evangelist rating

**Kin Score 29.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 21.1 |
| Developer ergonomics | 45.2 |
| Access clarity | 44.7 |

**Agent readiness 16.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |

**Regulatory alignment 23.1** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fca-uk/](https://apis.io/providers/fca-uk/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Financial Conduct Authority: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fca-uk/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
