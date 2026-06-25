# GoodData (gooddata)

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
