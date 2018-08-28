---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Add a new Team
  version: 1.0.0
  description: Add a new team.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/assignleadstopredefinedteams:
    put:
      summary: Assign InboundLead Todos to the predefined neg teams. e.g. Sales Valuers,
        Sales Viewings, Lettings Viewings etc etc
      description: Assign inboundlead todos to the predefined neg teams. e.g. sales
        valuers, sales viewings, lettings viewings etc etc.
      operationId: DefaultToDo_AssignLeadsToPredefinedTeamsBytoDoId
      x-api-path-slug: apitodoassignleadstopredefinedteams-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - Predefined
      - Neg
      - Teams
      - ""
      - E
      - G
      - ""
      - Sales
      - Valuers
      - ""
      - Sales
      - Viewings
      - ""
      - Lettings
      - Viewings
      - Etc
      - Etc
  /api/agency/teams:
    get:
      summary: Returns a list of team groups for the agency.
      description: Returns a list of team groups for the agency..
      operationId: Agency_TeamsBypageSizeBypageNumberByteamType
      x-api-path-slug: apiagencyteams-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Team
      - Groupsthe
      - Agency
  /api/event/{id}/setowningteam:
    put:
      summary: Changes the owning team of an event
      description: Changes the owning team of an event.
      operationId: Event_SetOwningTeamByidByteamId
      x-api-path-slug: apieventidsetowningteam-put
      parameters:
      - in: path
        name: id
        description: Event Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: Team Id for new owning team
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Owning
      - Team
      - Of
      - Event
  /api/group/{id}/setsearchteam:
    post:
      summary: Set the Team Group for a searching role
      description: Set the team group for a searching role.
      operationId: Group_SetSearchTeamByidBysetTeamCommandDataContract
      x-api-path-slug: apigroupidsetsearchteam-post
      parameters:
      - in: path
        name: id
        description: Group that owns the searching role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setTeamCommandDataContract
        description: Set Team Group Command
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Team
      - Groupa
      - Searching
      - Role
  /api/group/{id}/setteam:
    post:
      summary: Set the Groups owning team
      description: Set the groups owning team.
      operationId: Group_SetOwningTeamByidBysetTeamCommand
      x-api-path-slug: apigroupidsetteam-post
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setTeamCommand
        description: The set owning team data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Groups
      - Owning
      - Team
  /api/role/{id}/changeteam:
    put:
      summary: Change the owining team of a Role
      description: Change the owining team of a role.
      operationId: Role_ChangeTeamByidByteamId
      x-api-path-slug: apiroleidchangeteam-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Owining
      - Team
      - Of
      - Role
  /api/teams/{id}:
    get:
      summary: Gets a Team
      description: Gets a team.
      operationId: Teams_GetByid
      x-api-path-slug: apiteamsid-get
      parameters:
      - in: path
        name: id
        description: Id of Team
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Team
  /api/teams/add:
    post:
      summary: Add a new Team
      description: Add a new team.
      operationId: Teams_AddTeamBydataContract
      x-api-path-slug: apiteamsadd-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - New
      - Team
  /api/teams/{id}/members:
    get:
      summary: Gets the members of a team
      description: Gets the members of a team.
      operationId: Teams_MembersByid
      x-api-path-slug: apiteamsidmembers-get
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Members
      - Of
      - Team
  /api/teams/{id}/members/add:
    post:
      summary: Adds a member to a team
      description: Adds a member to a team.
      operationId: Teams_AddMemberByidByteamMemberCommands
      x-api-path-slug: apiteamsidmembersadd-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: teamMemberCommands
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Member
      - To
      - Team
  /api/teams/{id}/members/remove:
    post:
      summary: Remove a member from a team
      description: Remove a member from a team.
      operationId: Teams_RemoveMemberByidByremoveTeamMemberCommand
      x-api-path-slug: apiteamsidmembersremove-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: body
        name: removeTeamMemberCommand
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Member
      - From
      - Team
  /api/teams/{id}/setteamresponsibilities:
    put:
      summary: Sets the responsibilties for a team group
      description: Sets the responsibilties for a team group.
      operationId: Teams_SetTeamResponsibilitiesByidByresponsibities
      x-api-path-slug: apiteamsidsetteamresponsibilities-put
      parameters:
      - in: path
        name: id
      - in: body
        name: responsibities
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Responsibiltiesa
      - Team
      - Group
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