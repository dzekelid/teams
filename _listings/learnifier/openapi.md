swagger: "2.0"
x-collection-name: Learnifier
x-complete: 1
info:
  title: Learnifier
  version: 1.1.0
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