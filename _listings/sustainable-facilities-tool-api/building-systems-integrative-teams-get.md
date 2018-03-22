---
swagger: "2.0"
info:
  title: Sustainable Facilities Tool API
  description: Our core API allows developers to interact with the Sustainable Facilities
    Tool programmatically. It's designed for public use and to be easily integrated
    into other applications.
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
      description: Returns all building system integrative teams
      operationId: returnBuildingSystemIntegrativeTeams
      responses:
        200:
          description: Successful response
          schema:
            type: array
            items:
              $ref: '#/definitions/Building Systems'
      tags:
      - teams
definitions:
  Building Systems:
    properties:
      id:
        description: Returns a building system by Id. If an invalid Id is specified,
          a 404 (Not Found) code is returned.
        type: integer
      name:
        description: "string\tReturns a building system by name. If an invalid name
          is specified, a 404 (Not Found) code is returned."
        type: string
  Content Pages:
    properties:
      query:
        description: Returns content pages by full text search. If no pages are found,
          a 204 (No Content) code is returned.
        type: string
  FAR Clauses:
    properties:
      NAICS code:
        description: Returns any FAR clause number(s) and sample procurement langauge
          by NAICS code. If the NAICS code specified does not have any required clauses,
          a 404 (Not Found) code is returned.
        type: string
      id:
        description: Returns a content page by Id. If an invalid Id is specified,
          a 404 (Not Found) code is returned.
        type: integer
  Materials:
    properties:
      id:
        description: the id of the material
        type: string
      name:
        description: the name of the material
        type: string
  Products:
    properties:
      id:
        description: the id of the product
        type: string
      name:
        description: the name of the product
        type: string
  Services:
    properties:
      id:
        description: the id of the service
        type: string
      name:
        description: the name of the service
        type: string
  Tags:
    properties:
      id:
        description: the id of the tag
        type: string
      name:
        description: the name of the tag
        type: string
  Workspaces:
    properties:
      id:
        description: the id of the workspace
        type: string
      name:
        description: the name of the workspace
        type: string
x-collection-name: Sustainable Facilities Tool API
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