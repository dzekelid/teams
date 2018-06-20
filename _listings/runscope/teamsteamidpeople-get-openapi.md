---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 0
info:
  title: Runscope Get Teams People
  description: Teams Resource
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{teamId}/agents:
    get:
      summary: Get Teams Agents
      description: Team agents list
      operationId: teams.teamId.agents.get
      x-api-path-slug: teamsteamidagents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Agents
  /teams/{teamId}/integrations:
    get:
      summary: Get Teams Integrations
      description: Team integrations list
      operationId: teams.teamId.integrations.get
      x-api-path-slug: teamsteamidintegrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Integrations
  /teams/{teamId}/people:
    get:
      summary: Get Teams People
      description: Teams Resource
      operationId: teams.teamId.people.get
      x-api-path-slug: teamsteamidpeople-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - People
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