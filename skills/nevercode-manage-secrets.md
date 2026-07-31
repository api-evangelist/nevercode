---
name: Manage Codemagic secrets and environment variables
description: Create variable groups for an application and manage the environment variables (secrets) inside them.
api: openapi/nevercode-openapi-original.json
operations: ['ApiV3AppsAppIdVariableGroupsGetVariableGroups', 'ApiV3AppsAppIdVariableGroupsCreateVariableGroup', 'ApiV3VariableGroupsVariableGroupIdVariablesBulkImport', 'ApiV3VariableGroupsVariableGroupIdVariablesGetVariables']
---

# Manage Codemagic secrets and environment variables

## Authentication
Send your personal API token in the `x-auth-token` header on every request.

## Steps
1. List existing variable groups for an app with `ApiV3AppsAppIdVariableGroupsGetVariableGroups` (`GET /api/v3/apps/{app_id}/variable-groups`).
2. Create a new group with `ApiV3AppsAppIdVariableGroupsCreateVariableGroup` (`POST /api/v3/apps/{app_id}/variable-groups`).
3. Read the variables in a group with `ApiV3VariableGroupsVariableGroupIdVariablesGetVariables` (`GET /api/v3/variable-groups/{variable_group_id}/variables`).
4. Bulk-import variables with `ApiV3VariableGroupsVariableGroupIdVariablesBulkImport` (`POST /api/v3/variable-groups/{variable_group_id}/variables`).

## Conventions
- Mark sensitive variables as secure so their values are encrypted at rest.
- Errors are returned as JSON; handle 400 and 422 responses (see `errors/nevercode-problem-types.yml`).
