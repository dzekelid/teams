---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops Create an on-call override (take on-call)
  description: |-
    __NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__

    Replaces a currently on-call user on the team with another.

    This API may be called a maximum of 6 times per minute.
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v1/team:
    get:
      summary: List teams
      description: |-
        Get a list of teams for your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.get
      x-api-path-slug: apipublicv1team-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team
    post:
      summary: Add a team
      description: |-
        Add a team to your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.post
      x-api-path-slug: apipublicv1team-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Team
  /api-public/v1/team/{team}:
    delete:
      summary: Remove a team
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.delete
      x-api-path-slug: apipublicv1teamteam-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
    get:
      summary: Retrieve information for a team
      description: |-
        Get the information for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.get
      x-api-path-slug: apipublicv1teamteam-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
    put:
      summary: Update a team
      description: |-
        Update the designated team

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.put
      x-api-path-slug: apipublicv1teamteam-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be updated
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
  /api-public/v1/team/{team}/members:
    get:
      summary: Retrieve a list of members for a team
      description: |-
        Get the members for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.get
      x-api-path-slug: apipublicv1teamteammembers-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Members
    post:
      summary: Add a team member
      description: |-
        Add a team member to your team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.post
      x-api-path-slug: apipublicv1teamteammembers-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Members
  /api-public/v1/team/{team}/members/{user}:
    delete:
      summary: Remove a team member
      description: |-
        Remove a team from your organization.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.members.user.delete
      x-api-path-slug: apipublicv1teamteammembersuser-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to be deleted
      - in: path
        name: user
        description: The team member username
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Members
      - User
  /api-public/v1/team/{team}/oncall/schedule:
    get:
      summary: Get a team's on-call schedule
      description: |-
        __NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__

        Get the on-call schedule for a team, including on-call overrides.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.oncall.schedule.get
      x-api-path-slug: apipublicv1teamteamoncallschedule-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Oncall
      - Schedule
  /api-public/v1/team/{team}/oncall/user:
    patch:
      summary: Create an on-call override (take on-call)
      description: |-
        __NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__

        Replaces a currently on-call user on the team with another.

        This API may be called a maximum of 6 times per minute.
      operationId: api_public.v1.team.team.oncall.user.patch
      x-api-path-slug: apipublicv1teamteamoncalluser-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Oncall
      - User
  /api-public/v1/team/{team}/policies:
    get:
      summary: Retrieve a list of escalation policies for a team
      description: |-
        Get the escalation policies for the specified team.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v1.team.team.policies.get
      x-api-path-slug: apipublicv1teamteampolicies-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team to fetch
      responses:
        200:
          description: OK
      tags:
      - Team
      - Team
      - Policies
  /api-public/v2/team/{team}/oncall/schedule:
    get:
      summary: Get a team's on-call schedule
      description: |-
        Get the on-call schedule for a team, including on-call overrides.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v2.team.team.oncall.schedule.get
      x-api-path-slug: apipublicv2teamteamoncallschedule-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Api-public
      - V2
      - Team
      - Team
      - Oncall
      - Schedule
  /api-reporting/v1/team/{team}/oncall/log:
    get:
      summary: A list of shift changes for a team
      description: |-
        Returns a log of user shift changes for the specified team. This is historical
        data, and may be up to 15 minutes behind real-time log data.

        This API may be called a maximum of 6 times per minute.
      operationId: api_reporting.v1.team.team.oncall.log.get
      x-api-path-slug: apireportingv1teamteamoncalllog-get
      parameters:
      - in: query
        name: end
        description: Return shift changes occurring before this timestamp
      - in: query
        name: No Name
      - in: query
        name: start
        description: Return shift changes occurring after this timestamp
      - in: path
        name: team
        description: The VictorOps team slug
      - in: query
        name: userName
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Api-reporting
      - V1
      - Team
      - Team
      - Oncall
      - Log
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