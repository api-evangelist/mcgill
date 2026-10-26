# McGill University (mcgill)

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

McGill University is a public research university in Montreal, Quebec, Canada, and a member of the U15 group of Canadian research universities. This repository catalogs McGill's public, machine-readable footprint as an [APIs.json](https://apisjson.org) profile, and the operator of every surface is settled before it is catalogued. McGill operates exactly one machine-readable surface itself — the Shibboleth SAML 2.0 identity provider at `shibboleth.mcgill.ca`, whose federation metadata is served unauthenticated. Its research repository, research-data collection and course catalogue are real institutional facts but run as tenants on platforms McGill does not engineer (Scholaris, Borealis, CourseLeaf), and their contracts are recorded against those platforms, not against McGill.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=mcgill-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

University, Higher Education, Education, Canada, Quebec, U15, Public Research University, Identity Federation, Research Repository, Research Data, Course Catalog

## APIs

- **McGill University Authentication Service — Shibboleth SAML 2.0 Identity Provider** (`x-operator: institution`) — the one surface McGill itself operates. Federation metadata served unauthenticated at https://shibboleth.mcgill.ca/idp/shibboleth (HTTP 200, `application/xml`). Contract: [openapi/mcgill-shibboleth-idp-openapi.yml](openapi/mcgill-shibboleth-idp-openapi.yml)
- **eScholarship@McGill on Scholaris** (`x-operator: tenant`) — McGill's institutional repository on the Scholaris (Scholars Portal / OCUL) DSpace 7 platform. DSpace REST at https://mcgill.scholaris.ca/server/api and conformant OAI-PMH 2.0 at `/server/oai/request`. No contract saved: the interfaces are DSpace's.
- **McGill University Dataverse on Borealis** (`x-operator: tenant`) — McGill's research-data collection at https://borealisdata.ca/dataverse/mcgill. `borealisdata.ca` is a consortial host shared by six institutions in this catalog, so the Dataverse Native and Search contracts are not saved here.
- **McGill Course Catalogue on CourseLeaf** (`x-operator: tenant`) — https://coursecatalogue.mcgill.ca/, CNAMEd to `mcgill-ca-public.courseleaf.com`. Carries a live undocumented course-detail endpoint (`/ribbit/index.cgi?page=getcourse.rjs&code=COMP+202` → XML). No contract saved: the endpoint is CourseLeaf's product surface.

## Conformance

- [conformance/mcgill-conformance.yml](conformance/mcgill-conformance.yml) — `saml` and `shibboleth` evidenced institution-operated; `oai-pmh` evidenced tenant-operated.

## Authentication

- [authentication/mcgill-authentication.yml](authentication/mcgill-authentication.yml)

## Plans

- [plans/mcgill-plans-pricing.yml](plans/mcgill-plans-pricing.yml)

## Rate Limits

- [rate-limits/mcgill-rate-limits.yml](rate-limits/mcgill-rate-limits.yml)

## FinOps

- [finops/mcgill-finops.yml](finops/mcgill-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.mcgill.ca/
- Twitter: https://x.com/mcgillu
- LinkedIn: https://www.linkedin.com/school/mcgill-university/
- IdentityFederation: https://shibboleth.mcgill.ca/idp/shibboleth
- ResearchRepository: https://mcgill.scholaris.ca/
- OpenData: https://borealisdata.ca/dataverse/mcgill
- CourseCatalog: https://coursecatalogue.mcgill.ca/
- PrivacyPolicy: https://www.mcgill.ca/privacy-notice

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles who operates a
surface before any contract is saved. What changed and why:

- **Five OpenAPI documents describing the Dataverse Native and Search APIs on `borealisdata.ca`
  were removed, along with twenty-one artifacts derived from them** (JSON Schema, JSON Structure,
  examples, OpenCollection and Postman collections, Spectral rules, vocabulary, JSON-LD context,
  agentic-access, authentication). `borealisdata.ca` is a consortial host operated by Scholars
  Portal / OCUL and claimed by six institutions in this catalog; the contract is Dataverse's, not
  McGill's, and everything derived from it inherited that provenance. McGill's Dataverse
  *collection* is kept as a tenant relationship.
- **The Shibboleth identity provider was upgraded from a bare link to a catalogued contract.**
  Its SAML metadata (HTTP 200, `application/xml`, 8,995 bytes, entityID and `shibmd:Scope` both
  `mcgill.ca`, host resolving to 132.216.98.81 with no vendor CNAME) is the only machine-readable
  surface McGill itself operates.
- **The 2026-06-03 finding that eScholarship's OAI-PMH returned an SPA landing page was wrong.**
  That probe used the DSpace 6 path (`/oai/request`); the deployment is DSpace 7 and serves valid
  OAI-PMH 2.0 at https://mcgill.scholaris.ca/server/oai/request, with thirteen metadata prefixes.
  The endpoint was never dead — the path was.
- `coursecatalogue.mcgill.ca` sits on McGill's own domain but CNAMEs to
  `mcgill-ca-public.courseleaf.com`, so it is recorded as a tenant rather than as institution
  engineering, even though a host-only rule would read it as McGill's.
- Still absent, probed and confirmed: `api.mcgill.ca`, `data.mcgill.ca` and `opendata.mcgill.ca`
  do not resolve; `/llms.txt` and `/.well-known/security.txt` return 404; `github.com/mcgill` is
  an org with zero public repositories and no verifiable McGill ownership, so no GitHub pointer is
  asserted. `shibboleth.mcgill.ca/idp/status` returns 403 from the public internet.
- Minerva/Banner registration, WorldCat library discovery and Workday HR are behind authentication
  with no public interface.
- No endpoints were fabricated; every status code above was observed by direct probe.

## Maintainers

- Kin Lane — kin@apievangelist.com
