---
swagger: "2.0"
x-collection-name: PagerDuty
x-complete: 0
info:
  title: PagerDuty Add an escalation policy to a team
  version: 1.0.0
  description: Put teams  escalation policies escalation policy
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
    get:
      summary: List teams
      description: List teams of your PagerDuty account, optionally filtered by a
        search query.
      operationId: list-teams-of-your-pagerduty-account-optionally-filtered-by-a-search-query
      x-api-path-slug: teams-get
      parameters:
      - in: query
        name: query
        description: Filters the result, showing only the teams whose names or email
          addresses match the query
      responses:
        200:
          description: OK
      tags:
      - Teams
  /teams/{id}:
    get:
      summary: Get a team
      description: Get details about an existing team.
      operationId: get-details-about-an-existing-team
      x-api-path-slug: teamsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
    delete:
      summary: Delete a team
      description: Remove an existing team.
      operationId: remove-an-existing-team
      x-api-path-slug: teamsid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
    put:
      summary: Update a team
      description: Update an existing team.
      operationId: update-an-existing-team
      x-api-path-slug: teamsid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: team
        description: The team to be updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Teams
  /teams/{id}/escalation_policies/{escalation_policy_id}:
    delete:
      summary: Remove an escalation policy from a team
      description: Delete teams  escalation policies escalation policy
      operationId: remove-an-escalation-policy-from-a-team
      x-api-path-slug: teamsidescalation-policiesescalation-policy-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team Escalation Policies
    put:
      summary: Add an escalation policy to a team
      description: Put teams  escalation policies escalation policy
      operationId: add-an-escalation-policy-to-a-team
      x-api-path-slug: teamsidescalation-policiesescalation-policy-id-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team Escalation Policies
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