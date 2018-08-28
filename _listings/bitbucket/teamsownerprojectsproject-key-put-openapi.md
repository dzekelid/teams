---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Update Teams Owner Projects Project Key
  description: |-
    Since this endpoint can be used to both update and to create a
    project, the request body depends on the intent.

    ### Creation

    See the POST documentation for the project collection for an
    example of the request body.

    Note: The `key` should not be specified in the body of request
    (since it is already present in the URL). The `name` is required,
    everything else is optional.

    ### Update

    See the POST documentation for the project collection for an
    example of the request body.

    Note: The key is not required in the body (since it is already in
    the URL). The key may be specified in the body, if the intent is
    to change the key itself. In such a scenario, the location of the
    project is changed and is returned in the `Location` header of the
    response.
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
    parameters:
      summary: Parameters Teams Owner Projects
      description: Parameters teams owner projects
      operationId: parametersTeamsOwnerProjects
      x-api-path-slug: teamsownerprojects-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
    post:
      summary: Add Teams Owner Projects
      description: |-
        Creates a new project.

        Note that the avatar has to be embedded as either a data-url
        or a URL to an external image as shown in the examples below:

        ```
        $ body=$(cat << EOF
        {
            "name": "Mars Project",
            "key": "MARS",
            "description": "Software for colonizing mars.",
            "links": {
                "avatar": {
                    "href": "data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/..."
                }
            },
            "is_private": false
        }
        EOF
        )
        $ curl -H "Content-Type: application/json" \
               -X POST \
               -d "$body" \
               https://api.bitbucket.org/2.0/teams/teams-in-space/projects/ | jq .
        {
          // Serialized project document
        }
        ```

        or even:

        ```
        $ body=$(cat << EOF
        {
            "name": "Mars Project",
            "key": "MARS",
            "description": "Software for colonizing mars.",
            "links": {
                "avatar": {
                    "href": "http://i.imgur.com/72tRx4w.gif"
                }
            },
            "is_private": false
        }
        EOF
        )
        $ curl -H "Content-Type: application/json" \
               -X POST \
               -d "$body" \
               https://api.bitbucket.org/2.0/teams/teams-in-space/projects/ | jq .
        {
          // Serialized project document
        }
        ```
      operationId: postTeamsOwnerProjects
      x-api-path-slug: teamsownerprojects-post
      parameters:
      - in: body
        name: _body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
  /teams/{owner}/projects/{project_key}:
    delete:
      summary: Delete Teams Owner Projects Project Key
      description: Delete teams owner projects project key
      operationId: deleteTeamsOwnerProjectsProjectKey
      x-api-path-slug: teamsownerprojectsproject-key-delete
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
      - Project
      - Key
    get:
      summary: Get Teams Owner Projects Project Key
      description: Get teams owner projects project key
      operationId: getTeamsOwnerProjectsProjectKey
      x-api-path-slug: teamsownerprojectsproject-key-get
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
      - Project
      - Key
    parameters:
      summary: Parameters Teams Owner Projects Project Key
      description: Parameters teams owner projects project key
      operationId: parametersTeamsOwnerProjectsProjectKey
      x-api-path-slug: teamsownerprojectsproject-key-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
      - Project
      - Key
    put:
      summary: Update Teams Owner Projects Project Key
      description: |-
        Since this endpoint can be used to both update and to create a
        project, the request body depends on the intent.

        ### Creation

        See the POST documentation for the project collection for an
        example of the request body.

        Note: The `key` should not be specified in the body of request
        (since it is already present in the URL). The `name` is required,
        everything else is optional.

        ### Update

        See the POST documentation for the project collection for an
        example of the request body.

        Note: The key is not required in the body (since it is already in
        the URL). The key may be specified in the body, if the intent is
        to change the key itself. In such a scenario, the location of the
        project is changed and is returned in the `Location` header of the
        response.
      operationId: putTeamsOwnerProjectsProjectKey
      x-api-path-slug: teamsownerprojectsproject-key-put
      parameters:
      - in: body
        name: _body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Owner
      - Projects
      - Project
      - Key
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