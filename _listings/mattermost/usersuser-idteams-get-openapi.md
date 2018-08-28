---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get a user's teams
  description: |-
    Get a list of teams that a user is on.
    ##### Permissions
    Must be authenticated as the user or have the `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams:
    get:
      summary: Get teams
      description: |-
        For regular users only returns open teams. Users with the "manage_system" permission will return teams regardless of type. The result is based on query string parameters - page and per_page.
        ##### Permissions
        Must be authenticated. "manage_system" permission is required to show all teams.
      operationId: for-regular-users-only-returns-open-teams-users-with-the-manage-system-permission-will-return-teams-
      x-api-path-slug: teams-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of teams per page
      responses:
        200:
          description: OK
      tags:
      - Teams
  /teams/search:
    post:
      summary: Search teams
      description: |-
        Search teams based on search term provided in the request body.
        ##### Permissions
        Logged in user only shows open teams
        Logged in user with "manage_system" permission shows all teams
      operationId: search-teams-based-on-search-term-provided-in-the-request-body-permissionslogged-in-user-only-shows-
      x-api-path-slug: teamssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Teams
  /users/{user_id}/teams:
    get:
      summary: Get a user's teams
      description: |-
        Get a list of teams that a user is on.
        ##### Permissions
        Must be authenticated as the user or have the `manage_system` permission.
      operationId: get-a-list-of-teams-that-a-user-is-on-permissionsmust-be-authenticated-as-the-user-or-have-the-manag
      x-api-path-slug: usersuser-idteams-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Teams
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---