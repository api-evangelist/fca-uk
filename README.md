# Financial Conduct Authority (fca-uk)

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

## Insurance API posture

This is a regulator record, not a carrier record. The honest findings as of 2026-07-25:

- **No insurance API.** The FCA publishes no quote, bind, issue or FNOL surface, and no insurance product or claims API. That is expected — it does not underwrite.
- **One real public API.** The Financial Services Register API is genuine, free and self-serve, but its documentation is behind a Salesforce registration login and no OpenAPI definition is published.
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
