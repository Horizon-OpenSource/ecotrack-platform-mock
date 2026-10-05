# EcoTrack Platform - Mock API

Shared mock REST API for the EcoTrack Frontend Web Application.

This project follows the same `json-server` structure used by the course learning-center mock example. During Sprint 2 it provides temporary REST resources while the Spring Boot Web Services are not yet implemented.

## Run locally

```bash
npm install
npm start
```

Default URL: `http://localhost:3000`

Health endpoint:

```text
GET http://localhost:3000/api/v1/health
```

## Organization Management resources

```text
GET    /api/v1/organizations
GET    /api/v1/organizations/1
POST   /api/v1/organizations
PUT    /api/v1/organizations/1
PATCH  /api/v1/organizations/1

GET    /api/v1/sites?organizationId=1
POST   /api/v1/sites
PUT    /api/v1/sites/:id
PATCH  /api/v1/sites/:id
DELETE /api/v1/sites/:id

GET    /api/v1/business-units?organizationId=1
POST   /api/v1/business-units
PUT    /api/v1/business-units/:id
PATCH  /api/v1/business-units/:id
DELETE /api/v1/business-units/:id

GET    /api/v1/organization-activities?organizationId=1
```

Additional bounded-context resources will be added to the same `db.json` as the remaining EcoTrack frontend branches are integrated.
