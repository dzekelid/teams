swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 1
info:
  title: Sustainable Facilities Tool API
  description: our-core-api-allows-developers-to-interact-with-the-sustainable-facilities-tool-programmatically--its-designed-for-public-use-and-to-be-easily-integrated-into-other-applications-
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