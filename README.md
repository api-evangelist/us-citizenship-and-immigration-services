# US Citizenship and Immigration Services

The US Citizenship and Immigration Services (USCIS) is a government agency responsible for overseeing lawful immigration to the United States. USCIS provides a public developer portal (developer.uscis.gov) through its Torch API Program, offering OAuth 2.0-secured APIs for case status lookup and FOIA request submission to enable immigration case management software integration.

**Human URL:** [https://developer.uscis.gov](https://developer.uscis.gov)

## Scope

- **Type:** Contract
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
- **Modified:** 2026-05-03

## APIs

### USCIS Case Status API

Provides immigration case status information by receipt number. Returns current status, form type, historical timeline in English and Spanish. Rate limits: 5 TPS, 1,000 daily requests.

- **Base URL:** `https://api-int.uscis.gov/case-status`
- **Documentation:** [developer.uscis.gov/api/case-status](https://developer.uscis.gov/api/case-status)
- **Developer Portal:** [developer.uscis.gov](https://developer.uscis.gov/)

#### Properties

- [Documentation](https://developer.uscis.gov/api/case-status)
- [OpenAPI](openapi/uscis-case-status-api-openapi.yml)
- [DeveloperPortal](https://developer.uscis.gov/)
- [Sandbox](https://developer.uscis.gov/get-started/sandbox)

### USCIS FOIA Request and Status API

Enables submission of Freedom of Information Act (FOIA) and Privacy Act requests for Alien File records and status tracking of submitted requests. Version 1.2.0.

- **Base URL:** `https://api-int.uscis.gov/foia`
- **Documentation:** [developer.uscis.gov/api/foia-request-and-status](https://developer.uscis.gov/api/foia-request-and-status)

#### Properties

- [Documentation](https://developer.uscis.gov/api/foia-request-and-status)
- [OpenAPI](openapi/uscis-foia-api-openapi.yml)
- [DeveloperPortal](https://developer.uscis.gov/)

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [uscis-case-status-api-openapi.yml](openapi/uscis-case-status-api-openapi.yml) | USCIS Case Status API - case status lookup by receipt number |
| [uscis-foia-api-openapi.yml](openapi/uscis-foia-api-openapi.yml) | USCIS FOIA Request and Status API - submit and track FOIA requests |

### JSON Schemas

| Schema | Description |
|--------|-------------|
| [uscis-case-status-schema.json](json-schema/uscis-case-status-schema.json) | Schema for USCIS case status response including receipt number, form type, and historical timeline |

### JSON Structures

| Structure | Description |
|-----------|-------------|
| [uscis-case-status-structure.json](json-structure/uscis-case-status-structure.json) | Hierarchical structure documentation for USCIS case status API responses |

### JSON-LD Contexts

| Context | Description |
|---------|-------------|
| [us-citizenship-and-immigration-services-context.jsonld](json-ld/us-citizenship-and-immigration-services-context.jsonld) | Linked data context mapping USCIS concepts to schema.org and Dublin Core |

### Examples

| Example | Description |
|---------|-------------|
| [uscis-get-case-status-example.json](examples/uscis-get-case-status-example.json) | GET request retrieving a complete I-485 case status with historical timeline |
| [uscis-submit-foia-request-example.json](examples/uscis-submit-foia-request-example.json) | POST request submitting a FOIA request for Alien File records |

### Spectral Rules

| Ruleset | Description |
|---------|-------------|
| [uscis-api-rules.yml](rules/uscis-api-rules.yml) | Spectral linting rules enforcing USCIS API conventions |

### Naftiko Capabilities

**Shared Definitions:**

| File | Description |
|------|-------------|
| [capabilities/shared/uscis-case-status-api.yaml](capabilities/shared/uscis-case-status-api.yaml) | Shared capability definition for the USCIS Case Status API |
| [capabilities/shared/uscis-foia-api.yaml](capabilities/shared/uscis-foia-api.yaml) | Shared capability definition for the USCIS FOIA Request and Status API |

**Workflow Capabilities:**

| Capability | APIs | Description |
|-----------|------|-------------|
| [capabilities/immigration-case-management.yaml](capabilities/immigration-case-management.yaml) | Case Status API + FOIA API | Unified immigration case management for attorneys and software providers |

### Vocabulary

| File | Description |
|------|-------------|
| [us-citizenship-and-immigration-services-vocabulary.yml](vocabulary/us-citizenship-and-immigration-services-vocabulary.yml) | Domain vocabulary covering USCIS form types, case statuses, service centers, and immigration terminology |

## Authentication

All USCIS Torch APIs use OAuth 2.0 Client Credentials flow:

1. Register at [developer.uscis.gov](https://developer.uscis.gov/)
2. Create a Team App to receive `client_id` and `client_secret`
3. Exchange credentials for a Bearer token (30-minute expiry) at `https://api-int.uscis.gov/oauth/accesstoken`
4. Include `Authorization: Bearer {token}` in all API requests

## Common USCIS Form Types

| Form | Description |
|------|-------------|
| I-485 | Application to Register Permanent Residence or Adjust Status |
| I-130 | Petition for Alien Relative |
| I-765 | Application for Employment Authorization |
| I-90 | Application to Replace Permanent Resident Card |
| N-400 | Application for Naturalization |
| I-140 | Immigrant Petition for Alien Workers |
| I-539 | Application to Extend/Change Nonimmigrant Status |

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
