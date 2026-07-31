---
name: Inspect Codemagic applications and builds
description: List the applications available to the authenticated user and inspect the status, actions, and details of a specific build.
api: openapi/nevercode-openapi-original.json
operations: ['ApiV3UserAppsGetApps', 'ApiV3BuildsBuildIdGetBuild', 'ApiV3BuildsBuildIdActionsGetBuildActions']
---

# Inspect Codemagic applications and builds

Use the Codemagic REST API (v3) to see which apps you can access and to inspect a build.

## Authentication
Send your personal API token in the `x-auth-token` header on every request. Manage the token in Codemagic Account settings.

## Steps
1. Call `ApiV3UserAppsGetApps` (`GET /api/v3/user/apps`) to list the applications available to the authenticated user. Note the `app_id` of the app you care about.
2. For a known build, call `ApiV3BuildsBuildIdGetBuild` (`GET /api/v3/builds/{build_id}`) to read the build status and metadata.
3. Call `ApiV3BuildsBuildIdActionsGetBuildActions` (`GET /api/v3/builds/{build_id}/actions`) to see the actions/steps for that build.

## Conventions
- Base path is `/api/v3` on `https://codemagic.io`.
- Errors are returned as JSON; handle 400 (bad request) and 422 (validation) responses (see `errors/nevercode-problem-types.yml`).
