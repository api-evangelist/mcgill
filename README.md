# McGill University (mcgill)

McGill University is a public research university in Montreal, Quebec, Canada, ranked #64 in the QS World University Rankings 2025. This repository catalogs McGill's public, machine-readable developer and API footprint as an [APIs.json](https://apisjson.org) profile. McGill's strongest verifiable public API surface is its research-data infrastructure (the McGill University Dataverse on the Borealis platform) plus a Shibboleth SAML single sign-on identity service; most other systems are gated behind authentication or web UIs.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=mcgill-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Data, Canada, Quebec

## APIs

- **McGill University Dataverse (Borealis) - Native API** — Dataverse Native REST API over the McGill collection. Docs: https://borealisdata.ca/guides/en/latest/api/native-api.html (base: `https://borealisdata.ca/api`)
- **McGill University Dataverse (Borealis) - Search API** — Dataverse Search REST API. Docs: https://guides.dataverse.org/en/latest/api/search.html (base: `https://borealisdata.ca/api/search`)
- **McGill Shibboleth SAML Single Sign-On** — McGill Authentication Service, a SAML 2.0 Shibboleth IdP (identity/SSO, not an open data API). https://shibboleth.mcgill.ca/

## Plans

- [plans/mcgill-plans-pricing.yml](plans/mcgill-plans-pricing.yml)

## Rate Limits

- [rate-limits/mcgill-rate-limits.yml](rate-limits/mcgill-rate-limits.yml)

## FinOps

- [finops/mcgill-finops.yml](finops/mcgill-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.mcgill.ca/
- Twitter: https://twitter.com/mcgillu
- LinkedIn: https://www.linkedin.com/school/mcgill-university/
- Authentication: https://shibboleth.mcgill.ca/

## Notes

Verification caveats (probed 2026-06-03):

- The Borealis Dataverse Native and Search APIs were confirmed live — `GET /api/dataverses/mcgill` returned a McGill collection JSON record and `/api/search` returned HTTP 200.
- An Azure API Management developer-portal hostname (`mcgilluniversity.portal.azure-api.net`) appeared in search but did not resolve (connection refused), so it is not cataloged.
- A `github.com/mcgill` org exists but has zero public repositories and could not be verified as officially McGill-owned; `github.com/mcgillu` returned 404. No GitHub pointer is asserted in `apis.yml`.
- An eScholarship OAI-PMH path returned a single-page-app HTML landing page rather than valid OAI-PMH XML; no working public OAI-PMH endpoint was confirmed.
- Course catalogue and Minerva/Banner registration are web UIs without documented public APIs.
- No endpoints were fabricated; only live-verified surfaces are included.

## Maintainers

- Kin Lane — kin@apievangelist.com
