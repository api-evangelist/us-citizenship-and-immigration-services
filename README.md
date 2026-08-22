# US Citizenship and Immigration Services (us-citizenship-and-immigration-services)

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

The US Citizenship and Immigration Services (USCIS) is a government agency responsible for overseeing lawful immigration to the United States. Its primary function is to process and adjudicate applications for various immigration benefits, such as green cards, work permits, and naturalization. USCIS provides a public developer portal (developer.uscis.gov) with APIs for case status lookup and FOIA request submission. The Torch API Program enables qualified software developers to integrate USCIS services into immigration case management applications, providing OAuth 2.0 secured access to case status information and Freedom of Information Act (FOIA) request capabilities.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Federal Government
- Immigration
- Citizenship
- Case Status
- FOIA

## Timestamps

- **Created:** 2024-12-03
- **Modified:** 2026-05-19

## APIs

### USCIS Case Status API

The USCIS Case Status API provides case status information to USCIS customers and their representatives who require regular access to case status information. It accepts a 13-character USCIS receipt number and returns the current case status, form type, submission date, and historical status timeline in English and Spanish. Authentication uses OAuth 2.0 client credentials flow. Rate limits: 5 transactions per second, 1,000 daily requests.

- **Human URL:** [https://developer.uscis.gov/api/case-status](https://developer.uscis.gov/api/case-status)
- **Base URL:** `https://api-int.uscis.gov/case-status`

#### Tags

- Federal Government
- Immigration
- Case Status
- USCIS

#### Properties

- [Documentation](https://developer.uscis.gov/api/case-status)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-case-status-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Developer Portal](https://developer.uscis.gov/)
- [Sandbox](https://developer.uscis.gov/get-started/sandbox)
- [Authentication](https://developer.uscis.gov/article/how-get-access-tokens-client-credentials)
- [Postman Collection](collections/uscis-case-status-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uscis-case-status-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uscis-foia-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uscis-foia-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USCIS FOIA Request and Status API

The USCIS FOIA Request and Status API enables consumers to submit Freedom of Information Act (FOIA) or Privacy Act (PA) requests for Alien File records and check the status of submitted requests using the Request Number returned upon creation. Authentication uses OAuth 2.0 client credentials. Version 1.2.0 is the current production version.

- **Human URL:** [https://developer.uscis.gov/api/foia-request-and-status](https://developer.uscis.gov/api/foia-request-and-status)
- **Base URL:** `https://api-int.uscis.gov/foia`

#### Tags

- Federal Government
- Immigration
- FOIA
- Alien File
- Privacy Act
- USCIS

#### Properties

- [Documentation](https://developer.uscis.gov/api/foia-request-and-status)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-foia-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Developer Portal](https://developer.uscis.gov/)
- [Postman Collection](collections/uscis-case-status-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uscis-case-status-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/uscis-foia-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/uscis-foia-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/uscis)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
