# US Citizenship and Immigration Services (us-citizenship-and-immigration-services)

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
