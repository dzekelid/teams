---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Create a team
  version: 1.0.0
  description: Create a new team.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams:
    post:
      summary: Create a team
      description: Create a new team.
      operationId: create-a-new-team
      x-api-path-slug: teams-post
      parameters:
      - in: body
        name: team
        description: The team to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
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