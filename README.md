# Financial Conduct Authority (fca-uk)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The Financial Conduct Authority (FCA) is the United Kingdom's conduct regulator for around 42,000 financial services firms and the prudential regulator for most non-bank firms, operating alongside the Prudential Regulation Authority under the dual-regulation model. In insurance the FCA owns conduct regulation of general insurance and protection markets through ICOBS and the Consumer Duty, authorises and supervises insurers, Lloyd's managing agents, MGAs, brokers and appointed representatives, and publishes market-wide insurance data such as the annual General Insurance Value Measures.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fca-uk/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fca-uk/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Regulator
- Market Infrastructure
- Financial Services
- Public Register
- Conduct Regulation
- Open Finance
- Insurance Intermediaries
- Risk Data

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

### FCA Financial Services Register API

Read-only REST API over the Financial Services Register, the FCA's public record of authorised firms, individuals, funds and appointed representatives. Resources are addressed by Firm Reference Number, Individual Reference Number or Product Reference Number and expose sub-resources for names, individuals, permissions, requirements, passports, regulators, appointed representatives, addresses, waivers, exclusions and disciplinary history — the permissions data being where insurance authorisations (insurance distribution, insurance mediation, Lloyd's market activity) surface. Registration is free and self-serve, but the developer portal and its reference documentation are behind a Salesforce login; authentication is by `X-Auth-Email` and `X-Auth-Key` request headers. No OpenAPI or Swagger definition is published by the FCA.

- **Human URL:** [https://register.fca.org.uk/Developer/s/](https://register.fca.org.uk/Developer/s/)
- **Base URL:** `https://register.fca.org.uk/services/V0.1`

#### Tags

- Public Register
- Regulator
- Authorisation
- Firm Data
- United Kingdom

#### Properties

- [Documentation](https://www.fca.org.uk/firms/financial-services-register)
- [API Reference](https://register.fca.org.uk/Developer/s/)
- [Website](https://register.fca.org.uk/s/)

### FCA Data Publication API (FIRDS / FITRS)

Anonymous machine-to-machine query interface over the file artefacts published through data.fca.org.uk, documented in the FCA's own FIRDS and FITRS technical specifications. It is an OpenSearch/Elasticsearch query-string search — the index name is the resource, and the FCA supports a documented subset of the query_string DSL (`q`, `from`, `size`, `sort`, `pretty`, `df`, `default_operator`). Two indices respond publicly: `fca_data_firds_files` (UK instrument reference data, 11,583 records) and `fca_data_fitrs_files` (UK transparency calculation results, 2,603 records). Every other index name probed returns 403. No credentials, no OpenAPI. Markets reference data, not insurance data.

- **Human URL:** [https://data.fca.org.uk/#/download](https://data.fca.org.uk/#/download)
- **Base URL:** `https://api.data.fca.org.uk`

#### Properties

- [Documentation — FCA FIRDS technical specification](https://www.fca.org.uk/publication/systems-information/fca-firds-tech-spec.pdf)
- [API Reference — FCA FITRS technical specification](https://www.fca.org.uk/publication/systems-information/fca-fitrs-tech-spec.pdf)
- [Website](https://data.fca.org.uk/)

## Artifacts

Captured by the API Evangelist enrichment pipeline on 2026-07-25. No OpenAPI, GraphQL, AsyncAPI, gRPC, webhook, SDK, CLI, sandbox, Postman collection, MCP server or agent skill exists on any FCA property, so none is fabricated here.

- [Authentication profile](authentication/fca-uk-authentication.yml) — X-Auth-Email/X-Auth-Key on the Register API, anonymous on the data publication API
- [API conventions](conventions/fca-uk-conventions.yml)
- [Error catalog](errors/fca-uk-problem-types.yml) — observed error envelopes, not RFC 9457
- [Rate limits](rate-limits/fca-uk-rate-limits.yml)
- [Lifecycle](lifecycle/fca-uk-lifecycle.yml) — no SLA, no status page, no deprecation policy
- [Conformance](conformance/fca-uk-conformance.yml)
- [Data model](data-model/fca-uk-data-model.yml)
- [Packages](packages/fca-uk-packages.yml) — community clients only; the FCA ships no SDK
- [Well-known surface](well-known/fca-uk-well-known.yml) + [OIDC discovery](well-known/fca-uk-openid-configuration.json) (portal login, not the API)
- [Domain security probe](security/fca-uk-domain-security.yml)
- [llms.txt](llms/fca-uk-llms.txt)

## Insurance API posture

This is a regulator record, not a carrier record. The honest findings as of 2026-07-25:

- **No insurance API.** The FCA publishes no quote, bind, issue or FNOL surface, and no insurance product or claims API. That is expected — it does not underwrite.
- **Two real public APIs, neither about insurance products.** The Financial Services Register API is genuine, free and self-serve, but its documentation is behind a Salesforce registration login. The FIRDS/FITRS data publication API is anonymous and documented in FCA technical specifications, but it publishes markets reference data. Neither has an OpenAPI definition.
- **No ACORD.** A site search of fca.org.uk for "ACORD" returns zero results. The FCA does not reference ACORD, AL3, ACORD XML or NGDS anywhere in its published material.
- **No open-insurance mandate.** The FCA's *Open finance: our vision for a smart data future* roadmap (14 April 2026) names insurance as an in-scope sector, but it is a roadmap and not a rule; the formal discussion paper on the first scheme is not due until Q4 2026.
- **Insurance data is spreadsheets.** General Insurance Value Measures data is published as XLSX downloads, not as an API.

## Common Properties

- [Website](https://www.fca.org.uk/)
- [Documentation](https://www.fca.org.uk/firms/financial-services-register)
- [Handbook](https://handbook.fca.org.uk/)
- [Data](https://www.fca.org.uk/data)
- [Registers](https://data.fca.org.uk/)
- [LinkedIn](https://www.linkedin.com/company/financial-conduct-authority)
- [Blog](https://www.fca.org.uk/news)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
