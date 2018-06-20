---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Get Teams Team Members Username
  description: |-
    The "Get team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Get team membership API instead. It allows you to get both active and pending memberships.

    Get team member.
    In order to get if a user is a member of a team, the authenticated user mus
    be a member of the team.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orgs/{org}/teams:
    get:
      summary: Get Orgs Org Teams
      description: List teams.
      operationId: list-teams
      x-api-path-slug: orgsorgteams-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Teams
    post:
      summary: Add Orgs Org Teams
      description: |-
        Create team.
        In order to create a team, the authenticated user must be an owner of organization.
      operationId: create-teamin-order-to-create-a-team-the-authenticated-user-must-be-an-owner-of-organization
      x-api-path-slug: orgsorgteams-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: org
        description: Name of organisation
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Teams
  /repos/{owner}/{repo}/teams:
    get:
      summary: Get Repos Owner Repo Teams
      description: Get list of teams
      operationId: get-list-of-teams
      x-api-path-slug: reposownerrepoteams-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Teams
  /teams/{teamId}:
    delete:
      summary: Delete Teams Team
      description: |-
        Delete team.
        In order to delete a team, the authenticated user must be an owner of the
        org that the team is associated with.
      operationId: delete-teamin-order-to-delete-a-team-the-authenticated-user-must-be-an-owner-of-theorg-that-the-team
      x-api-path-slug: teamsteamid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
    get:
      summary: Get Teams Team
      description: Get team.
      operationId: get-team
      x-api-path-slug: teamsteamid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
    patch:
      summary: Patch Teams Team
      description: |-
        Edit team.
        In order to edit a team, the authenticated user must be an owner of the org
        that the team is associated with.
      operationId: edit-teamin-order-to-edit-a-team-the-authenticated-user-must-be-an-owner-of-the-orgthat-the-team-is-
      x-api-path-slug: teamsteamid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: teamId
        description: Id of team
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
  /teams/{teamId}/members:
    get:
      summary: Get Teams Team Members
      description: |-
        List team members.
        In order to list members in a team, the authenticated user must be a member
        of the team.
      operationId: list-team-membersin-order-to-list-members-in-a-team-the-authenticated-user-must-be-a-memberof-the-te
      x-api-path-slug: teamsteamidmembers-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Members
  /teams/{teamId}/members/{username}:
    delete:
      summary: Delete Teams Team Members Username
      description: |-
        The "Remove team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Remove team membership API instead. It allows you to remove both active and pending memberships.

        Remove team member.
        In order to remove a user from a team, the authenticated user must have 'admin'
        permissions to the team or be an owner of the org that the team is associated
        with.
        NOTE This does not delete the user, it just remove them from the team.
      operationId: the-remove-team-member-api-is-deprecated-and-is-scheduled-for-removal-in-the-next-major-version-of-t
      x-api-path-slug: teamsteamidmembersusername-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      - in: path
        name: username
        description: Name of a member
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Members
      - Username
    get:
      summary: Get Teams Team Members Username
      description: |-
        The "Get team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Get team membership API instead. It allows you to get both active and pending memberships.

        Get team member.
        In order to get if a user is a member of a team, the authenticated user mus
        be a member of the team.
      operationId: the-get-team-member-api-is-deprecated-and-is-scheduled-for-removal-in-the-next-major-version-of-the-
      x-api-path-slug: teamsteamidmembersusername-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      - in: path
        name: username
        description: Name of a member
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Members
      - Username
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