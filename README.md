# GoodData (gooddata)

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

GoodData is an analytics and business intelligence platform for building and embedding interactive dashboards, metrics, and self-service analytics. GoodData Cloud exposes a full REST API (Entity, Declarative, and Action APIs) for managing workspaces, data sources, the logical data model, metrics, visualizations, dashboards, AFM executions, users, and permissions, authenticated with a Bearer API token.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/apis.yml)

## Tags

- Analytics
- Business Intelligence
- Embedded Analytics
- Dashboards
- Data

## Timestamps

- **Created:** 2026-06-21

## APIs

### GoodData Workspaces API

Create, read, update, and delete workspaces and workspace settings through the Entity API, supporting hierarchical and multi-tenant workspace structures at /api/v1/entities/workspaces.

- **Human URL:** [https://www.gooddata.com/docs/cloud/create-workspaces/entity-interface/](https://www.gooddata.com/docs/cloud/create-workspaces/entity-interface/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Workspaces
- Tenants
- Entities

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/create-workspaces/entity-interface/)
- [API Reference](https://www.gooddata.com/docs/cloud/api-and-sdk/api/api_reference_all/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Data Sources API

Register and manage connections to data warehouses and databases via /api/v1/entities/dataSources, with connection testing through the Action API at /api/v1/actions/dataSources/{dataSourceId}/test.

- **Human URL:** [https://www.gooddata.com/docs/cloud/connect-data/manage-data-sources/](https://www.gooddata.com/docs/cloud/connect-data/manage-data-sources/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Data Sources
- Connections
- Databases

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/connect-data/manage-data-sources/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Logical Data Model API

Retrieve and set the workspace logical data model (datasets, attributes, facts, references) as an all-in-one declarative document at /api/v1/layout/workspaces/{workspaceId}/logicalModel.

- **Human URL:** [https://www.gooddata.com/docs/cloud/create-workspaces/declarative-interface/](https://www.gooddata.com/docs/cloud/create-workspaces/declarative-interface/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- LDM
- Logical Data Model
- Declarative

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/create-workspaces/declarative-interface/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Metrics API

Define and manage reusable MAQL metrics within a workspace through the Entity API at /api/v1/entities/workspaces/{workspaceId}/metrics.

- **Human URL:** [https://www.gooddata.com/docs/cloud/create-metrics/create-metrics-using-api/](https://www.gooddata.com/docs/cloud/create-metrics/create-metrics-using-api/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Metrics
- MAQL
- Measures

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/create-metrics/create-metrics-using-api/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Visualizations & Dashboards API

Manage visualization objects (insights) and analytical dashboards via /api/v1/entities/workspaces/{workspaceId}/visualizationObjects and /analyticalDashboards.

- **Human URL:** [https://www.gooddata.com/docs/cloud/create-dashboards/](https://www.gooddata.com/docs/cloud/create-dashboards/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Visualizations
- Dashboards
- Insights

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/create-dashboards/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Execution / AFM API

Run analytical computations using the AFM (Analytical Foundation Model) via POST /api/v1/actions/workspaces/{workspaceId}/execution/afm/execute and retrieve paged results from the corresponding result endpoint.

- **Human URL:** [https://www.gooddata.ai/docs/cloud/api-and-sdk/api/access_raw_data_through_api/](https://www.gooddata.ai/docs/cloud/api-and-sdk/api/access_raw_data_through_api/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Execution
- AFM
- Reporting

#### Properties

- [Documentation](https://www.gooddata.ai/docs/cloud/api-and-sdk/api/access_raw_data_through_api/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GoodData Users & Permissions API

Manage users, user groups, and workspace permissions via /api/v1/entities/users, /api/v1/entities/userGroups, and workspace permission endpoints under the organization.

- **Human URL:** [https://www.gooddata.com/docs/cloud/manage-organization/organization-api/](https://www.gooddata.com/docs/cloud/manage-organization/organization-api/)
- **Base URL:** `https://{domain}.gooddata.com/api/v1`

#### Tags

- Users
- Permissions
- Access Control

#### Properties

- [Documentation](https://www.gooddata.com/docs/cloud/manage-organization/organization-api/)
- [OpenAPI](openapi/gooddata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gooddata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gooddata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/gooddata)
- [LinkedIn](https://www.linkedin.com/company/gooddata)
- [Website](https://www.gooddata.com)
- [Documentation](https://www.gooddata.com/docs/cloud/)
- [Plans](plans/gooddata-plans-pricing.yml)
- [Rate Limits](rate-limits/gooddata-rate-limits.yml)
- [Fin Ops](finops/gooddata-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
