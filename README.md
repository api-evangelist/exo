# Exo

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

Exo (Exo Imaging, Inc.) is a Santa Clara, California medical imaging company building a handheld
ultrasound ecosystem for point-of-care ultrasound (POCUS). Its silicon-based Exo Iris handheld probe
pairs an FDA-cleared, on-device AI suite with Exo Works, an AWS-hosted POCUS workflow, documentation,
billing, QA and credentialing platform.

**Exo publishes no public developer API.** Contract discovery probed `/openapi.json`, `/openapi.yaml`,
`/swagger.json`, `/v1/openapi.json`, `/api-docs`, `/docs`, `/redoc`, `/graphql`, and the full
`/.well-known/` discovery surface across `www.exo.inc`, `support.exo.inc`, `cloud.exoworks.inc`,
`exoworks.inc` and `api.exoworks.inc` — every probe returned 404, 403, or a single-page-app HTML shell.
There is no OpenAPI, no GraphQL, no MCP server, no A2A agent card, no `llms.txt`, no published SDK, and
no developer portal. The production API host `api.prod.exoworks.inc` (AWS API Gateway) rejects anonymous
requests with HTTP 403 and is undocumented.

What Exo does publish is an **integration surface for hospital IT**: DICOM (any DICOM-enabled
ultrasound, modality worklist, PACS/VNA), HL7 v2 (ADT, ultrasound orders, exam results) on the Exo Works
Enterprise tier, SAML single sign-on and Active Directory, plus Epic App Orchard certification and
Oracle Cerner CODE program approval — captured in `conformance/` and `authentication/`.

- https://www.exo.inc/
- https://support.exo.inc/hc/en-us
- https://forgeglobal.com/exo_stock/ (secondary-market listing that surfaced this company)
