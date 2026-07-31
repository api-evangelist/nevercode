---
name: Inspect Codemagic over-the-air updates
description: Read over-the-air (OTA) update account info, list deployment releases, and list deployment keys for a project.
api: openapi/nevercode-openapi-original.json
operations: ['ApiV3OverTheAirUpdatesGetAccountInfo', 'ApiV3OverTheAirUpdatesDeploymentsDeploymentIdReleasesListDeploymentReleases', 'ApiV3OverTheAirUpdatesProjectsProjectIdDeploymentKeysListDeploymentKeys']
---

# Inspect Codemagic over-the-air updates

## Authentication
Send your personal API token in the `x-auth-token` header on every request.

## Steps
1. Read OTA account info with `ApiV3OverTheAirUpdatesGetAccountInfo` (`GET /api/v3/over-the-air-updates`).
2. List deployment keys for a project with `ApiV3OverTheAirUpdatesProjectsProjectIdDeploymentKeysListDeploymentKeys` (`GET /api/v3/over-the-air-updates/projects/{project_id}/deployment-keys`).
3. List releases for a deployment with `ApiV3OverTheAirUpdatesDeploymentsDeploymentIdReleasesListDeploymentReleases` (`GET /api/v3/over-the-air-updates/deployments/{deployment_id}/releases`).

## Conventions
- OTA endpoints are also aliased under `/api/v3/ota/...`.
- Errors are returned as JSON; handle 400 and 422 responses (see `errors/nevercode-problem-types.yml`).
