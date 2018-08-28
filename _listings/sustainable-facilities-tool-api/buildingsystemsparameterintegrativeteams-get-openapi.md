---
swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 0
info:
  title: Sustainable Facilities Tool API Building System Integrative Team
  description: Returns a building system integrative team by parameter.
  termsOfService: https://sftool.gov/developer/terms-of-use
  version: 1.0.0
host: api.data.gov
basePath: /sftool/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /building-systems/integrative-teams:
    get:
      summary: Building System Integrative Teams
      description: Returns all building system integrative teams.
      operationId: returnBuildingSystemIntegrativeTeams
      x-api-path-slug: buildingsystemsintegrativeteams-get
      responses:
        200:
          description: OK
      tags:
      - Teams
  /building-systems/{parameter}/integrative-teams:
    get:
      summary: Building System Integrative Team
      description: Returns a building system integrative team by parameter.
      operationId: returnBuildingSystemIntegrativeTeams
      x-api-path-slug: buildingsystemsparameterintegrativeteams-get
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