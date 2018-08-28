swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 1
info:
  title: Webex Teams API
  description: hey-there-thanks-for-checking-out-cisco-webex-for-developers--if-youve-used-cisco-webex-meetings-or-cisco-webex-teams-formerly-cisco-spark-you-know-how-easy-it-is-to-meet-and-collaborate-with-your-team-members-and-customers-the-webex-for-developers-program-opens-up-the-power-behind-the-webex-platform-to-anyone-seeking-to-extend-the-webex-experience-webex-meetings-is-a-powerful-conferencing-solution-that-lets-you-connect-with-anyone-anywhere-in-real-time--by-combining-video-audio-and-content-sharing-webex-meetings-creates-an-effective-conferencing-environment-leading-to-more-productive-meetings-and-increased-productivity--developer-information-for-webex-meetings-will-soon-be-available-on-this-site--in-the-meantime-to-get-started-with-developing-for-webex-meetings-please-see-the-getting-started-guides-over-on-cisco-devnet--keep-reading-for-information-about-webex-teams-webex-teams-makes-staying-in-sync-with-your-teammates-and-customers-easy-conversations-in-webex-teams-take-place-in-virtual-meeting-rooms--some-rooms-live-for-a-few-hours-while-others-become-permanent-fixtures-of-your-teams-workflow-with-titles-like-daily-standup-or-build-status--webex-teams-allows-conversations-to-flow-seamlessly-between-messages-video-calls-and-realtime-whiteboarding-sessions--no-other-solution-brings-together-so-many-facets-of-collaboration-into-a-single-unified-platform-httpsdeveloper-webex-comgettingstarted-html
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams:
    get:
      summary: List teams
      description: |-
        List teams.

        https://developer.webex.com/endpoint-teams-get.html
      operationId: TeamsGet
      x-api-path-slug: teams-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Teams
    post:
      summary: Create a team
      description: |-
        Create a new team.

        https://developer.webex.com/endpoint-teams-post.html
      operationId: TeamsPost2
      x-api-path-slug: teams-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
  /rooms:
    post:
      summary: Create a Team room
      description: |-
        Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

        https://developer.webex.com/endpoint-rooms-post.html
      operationId: RoomsPost5
      x-api-path-slug: rooms-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
  /rooms/{_room}:
    get:
      summary: Get Team room details
      description: "Shows details for a room, by ID.\r\n\r\nSpecify the room ID in
        the roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-get.html"
      operationId: RoomsByRoomGet2
      x-api-path-slug: rooms-room-get
      parameters:
      - in: path
        name: _room
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
      - Details
    delete:
      summary: Delete a Team room
      description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId
        parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
      operationId: RoomsByRoomDelete5
      x-api-path-slug: rooms-room-delete
      parameters:
      - in: path
        name: _room
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
  /team/memberships/{_membership}:
    get:
      summary: Get team membership details
      description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
        ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
      operationId: TeamMembershipsByMembershipGet
      x-api-path-slug: teammemberships-membership-get
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
      - Details
    put:
      summary: Update a team membership
      description: |-
        Updates properties for a membership by ID.

        Specify the membership ID in the membershipId URI parameter.

        https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
      operationId: TeamMembershipsByMembershipPut
      x-api-path-slug: teammemberships-membership-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
    delete:
      summary: Delete a team membership
      description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in
        the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
      operationId: TeamMembershipsByMembershipDelete
      x-api-path-slug: teammemberships-membership-delete
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
  /teams/{_team}:
    get:
      summary: Get team details
      description: |-
        Show details for a team.

        https://developer.webex.com/endpoint-teams-teamId-get.html
      operationId: TeamsByTeamGet
      x-api-path-slug: teams-team-get
      parameters:
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Details
    put:
      summary: Update a team
      description: |-
        Update a team.

        https://developer.webex.com/endpoint-teams-teamId-put.html
      operationId: TeamsByTeamPut
      x-api-path-slug: teams-team-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
    delete:
      summary: Delete a team
      description: |-
        Delete a team.

        https://developer.webex.com/endpoint-teams-teamId-delete.html
      operationId: TeamsByTeamDelete2
      x-api-path-slug: teams-team-delete
      parameters:
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
  /team/memberships:
    get:
      summary: List team memberships
      description: "Lists all team memberships. By default, lists memberships for
        teams to which the authenticated user belongs.\r\n\r\nUse query parameters
        to filter the response.\r\n\r\nUse teamId to list memberships for a team,
        by ID.\r\n\r\nUse either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
      operationId: TeamMembershipsGet
      x-api-path-slug: teammemberships-get
      parameters:
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Team
      - Memberships
    post:
      summary: Create a team membership
      description: |-
        Add someone to a team by Person ID or email address; optionally making them a moderator.

        https://developer.webex.com/endpoint-teammemberships-post.html
      operationId: TeamMembershipsPost
      x-api-path-slug: teammemberships-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership