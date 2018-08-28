---
swagger: "2.0"
x-collection-name: Learnifier
x-complete: 0
info:
  title: Learnifier Project team members
  version: 1.1.0
  description: Returns the project team members. A team member is a ....
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orgunits/{orgid}/projects/{projectid}/teammembers:
    get:
      summary: Project team members
      description: Returns the project team members. A team member is a ....
      operationId: orgunits.orgid.projects.projectid.teammembers.get
      x-api-path-slug: orgunitsorgidprojectsprojectidteammembers-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Team
      - Members
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