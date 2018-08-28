---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Get Teams Owner Projects
  description: Get teams owner projects
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams:
    get:
      summary: Get Teams
      description: |-
        Returns all the teams that the authenticated user is associated
        with.
      operationId: getTeams
      x-api-path-slug: teams-get
      parameters:
      - in: query
        name: role
        description: Filters the teams based on the authenticated users role on each
          team
      responses:
        200:
          description: OK
      tags:
      - Teams
    parameters:
      summary: Parameters Teams
      description: Parameters teams
      operationId: parametersTeams
      x-api-path-slug: teams-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
  /teams/{owner}/projects/:
    get:
      summary: Get Teams Owner Projects
      description: Get teams owner projects
      operationId: getTeamsOwnerProjects
      x-api-path-slug: teamsownerprojects-get
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
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