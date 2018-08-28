---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Remove user from team
  description: |-
    Delete the team member object for a user, effectively removing them from a team.
    ##### Permissions
    Must be logged in as the user or have the `remove_user_from_team` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams:
    get:
      summary: Get teams
      description: |-
        For regular users only returns open teams. Users with the "manage_system" permission will return teams regardless of type. The result is based on query string parameters - page and per_page.
        ##### Permissions
        Must be authenticated. "manage_system" permission is required to show all teams.
      operationId: for-regular-users-only-returns-open-teams-users-with-the-manage-system-permission-will-return-teams-
      x-api-path-slug: teams-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of teams per page
      responses:
        200:
          description: OK
      tags:
      - Teams
    post:
      summary: Create a team
      description: |-
        Create a new team on the system.
        ##### Permissions
        Must be authenticated and have the `create_team` permission.
      operationId: create-a-new-team-on-the-system-permissionsmust-be-authenticated-and-have-the-create-team-permission
      x-api-path-slug: teams-post
      parameters:
      - in: body
        name: body
        description: Team that is to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Team
  /teams/search:
    post:
      summary: Search teams
      description: |-
        Search teams based on search term provided in the request body.
        ##### Permissions
        Logged in user only shows open teams
        Logged in user with "manage_system" permission shows all teams
      operationId: search-teams-based-on-search-term-provided-in-the-request-body-permissionslogged-in-user-only-shows-
      x-api-path-slug: teamssearch-post
      parameters:
      - in: body
        name: body
        description: Search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - Teams
  /users/{user_id}/teams:
    get:
      summary: Get a user's teams
      description: |-
        Get a list of teams that a user is on.
        ##### Permissions
        Must be authenticated as the user or have the `manage_system` permission.
      operationId: get-a-list-of-teams-that-a-user-is-on-permissionsmust-be-authenticated-as-the-user-or-have-the-manag
      x-api-path-slug: usersuser-idteams-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Users
      - Teams
  /teams/{team_id}:
    get:
      summary: Get a team
      description: |-
        Get a team on the system.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-team-on-the-system-permissionsmust-be-authenticated-and-have-the-view-team-permission
      x-api-path-slug: teamsteam-id-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
    put:
      summary: Update a team
      description: |-
        Update a team by providing the team object. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
        ##### Permissions
        Must have the `manage_team` permission.
      operationId: update-a-team-by-providing-the-team-object-the-fields-that-can-be-updated-are-defined-in-the-request
      x-api-path-slug: teamsteam-id-put
      parameters:
      - in: body
        name: body
        description: Team to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
    delete:
      summary: Delete a team
      description: |-
        Soft deletes a team, by marking the team as deleted in the database. Soft deleted teams will not be accessible in the user interface.

        Optionally use the permanent query parameter to hard delete the team for compliance reasons.
        ##### Permissions
        Must have the `manage_team` permission.
      operationId: soft-deletes-a-team-by-marking-the-team-as-deleted-in-the-database-soft-deleted-teams-will-not-be-ac
      x-api-path-slug: teamsteam-id-delete
      parameters:
      - in: query
        name: permanent
        description: Permanently delete the team, to be used for compliance reasons
          only
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
  /teams/{team_id}/patch:
    put:
      summary: Patch a team
      description: |-
        Partially update a team by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
        ##### Permissions
        Must have the `manage_team` permission.
      operationId: partially-update-a-team-by-providing-only-the-fields-you-want-to-update-omitted-fields-will-not-be-u
      x-api-path-slug: teamsteam-idpatch-put
      parameters:
      - in: body
        name: body
        description: Team object that is to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
  /teams/name/{name}:
    get:
      summary: Get a team by name
      description: |-
        Get a team based on provided name string
        ##### Permissions
        Must be authenticated, team type is open and have the `view_team` permission.
      operationId: get-a-team-based-on-provided-name-string-permissionsmust-be-authenticated-team-type-is-open-and-have
      x-api-path-slug: teamsnamename-get
      parameters:
      - in: path
        name: name
        description: Team Name
      responses:
        200:
          description: OK
      tags:
      - Team
      - By
      - Name
  /teams/name/{name}/exists:
    get:
      summary: Check if team exists
      description: Check if the team exists based on a team name.
      operationId: check-if-the-team-exists-based-on-a-team-name
      x-api-path-slug: teamsnamenameexists-get
      parameters:
      - in: path
        name: name
        description: Team Name
      responses:
        200:
          description: OK
      tags:
      - Check
      - If
      - Team
      - Exists
  /teams/{team_id}/members:
    get:
      summary: Get team members
      description: |-
        Get a page team members list based on query string parameters - team id, page and per page.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-page-team-members-list-based-on-query-string-parameters--team-id-page-and-per-page-permissions
      x-api-path-slug: teamsteam-idmembers-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of users per page
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Members
    post:
      summary: Add user to team
      description: |-
        Add user to the team by user_id.
        ##### Permissions
        Must be authenticated and team be open to add self. For adding another user, authenticated user must have the `add_user_to_team` permission.
      operationId: add-user-to-the-team-by-user-id-permissionsmust-be-authenticated-and-team-be-open-to-add-self-for-ad
      x-api-path-slug: teamsteam-idmembers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Team
  /teams/members/invite:
    post:
      summary: Add user to team from invite
      description: |-
        Using either an invite id or hash/data pair from an email invite link, add a user to a team.
        ##### Permissions
        Must be authenticated.
      operationId: using-either-an-invite-id-or-hashdata-pair-from-an-email-invite-link-add-a-user-to-a-team-permission
      x-api-path-slug: teamsmembersinvite-post
      parameters:
      - in: query
        name: data
        description: Data with time and team id
      - in: query
        name: hash
        description: Hash value with time, team id and and InviteSaltId
      - in: query
        name: invite_id
        description: Invite id to add user to the team
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Team
      - From
      - Invite
  /teams/{team_id}/members/batch:
    post:
      summary: Add multiple users to team
      description: |-
        Add a number of users to the team by user_id.
        ##### Permissions
        Must be authenticated. Authenticated user must have the `add_user_to_team` permission.
      operationId: add-a-number-of-users-to-the-team-by-user-id-permissionsmust-be-authenticated-authenticated-user-mus
      x-api-path-slug: teamsteam-idmembersbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Users
      - To
      - Team
  /users/{user_id}/teams/members:
    get:
      summary: Get team members for a user
      description: |-
        Get a list of team members for a user. Useful for getting the ids of teams the user is on and the roles they have in those teams.
        ##### Permissions
        Must be logged in as the user or have the `edit_other_users` permission.
      operationId: get-a-list-of-team-members-for-a-user-useful-for-getting-the-ids-of-teams-the-user-is-on-and-the-rol
      x-api-path-slug: usersuser-idteamsmembers-get
      parameters:
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Membersa
      - User
  /teams/{team_id}/members/{user_id}:
    get:
      summary: Get a team member
      description: |-
        Get a team member on the system.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-team-member-on-the-system-permissionsmust-be-authenticated-and-have-the-view-team-permission
      x-api-path-slug: teamsteam-idmembersuser-id-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Member
    delete:
      summary: Remove user from team
      description: |-
        Delete the team member object for a user, effectively removing them from a team.
        ##### Permissions
        Must be logged in as the user or have the `remove_user_from_team` permission.
      operationId: delete-the-team-member-object-for-a-user-effectively-removing-them-from-a-team-permissionsmust-be-lo
      x-api-path-slug: teamsteam-idmembersuser-id-delete
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - User
      - From
      - Team
  /teams/{team_id}/members/ids:
    post:
      summary: Get team members by ids
      description: |-
        Get a list of team members based on a provided array of user ids.
        ##### Permissions
        Must have `view_team` permission for the team.
      operationId: get-a-list-of-team-members-based-on-a-provided-array-of-user-ids-permissionsmust-have-view-team-perm
      x-api-path-slug: teamsteam-idmembersids-post
      parameters:
      - in: body
        name: body
        description: List of user ids
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Members
      - By
      - Ids
  /teams/{team_id}/stats:
    get:
      summary: Get a team stats
      description: |-
        Get a team stats on the system.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-team-stats-on-the-system-permissionsmust-be-authenticated-and-have-the-view-team-permission
      x-api-path-slug: teamsteam-idstats-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Stats
  /teams/{team_id}/image:
    get:
      summary: Get the team icon
      description: |-
        Get the team icon of the team.

        __Minimum server version__: 4.9

        ##### Permissions
        User must be authenticated. In addition, team must be open or the user must have the `view_team` permission.
      operationId: get-the-team-icon-of-the-team-minimum-server-version--49-permissionsuser-must-be-authenticated-in-ad
      x-api-path-slug: teamsteam-idimage-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Icon
    post:
      summary: Sets the team icon
      description: |-
        Sets the team icon for the team.

        __Minimum server version__: 4.9

        ##### Permissions
        Must be authenticated and have the `manage_team` permission.
      operationId: sets-the-team-icon-for-the-team-minimum-server-version--49-permissionsmust-be-authenticated-and-have
      x-api-path-slug: teamsteam-idimage-post
      parameters:
      - in: formData
        name: image
        description: The image to be uploaded
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Team
      - Icon
  /teams/{team_id}/members/{user_id}/roles:
    put:
      summary: Update a team member roles
      description: |-
        Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
        ##### Permissions
        Must be authenticated and have the `manage_team_roles` permission.
      operationId: update-a-team-member-roles-valid-team-roles-are-team-user-team-admin-or-both-of-them-overwrites-any-
      x-api-path-slug: teamsteam-idmembersuser-idroles-put
      parameters:
      - in: body
        name: body
        description: Space-delimited team roles to assign to the user
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Member
      - Roles
  /users/{user_id}/teams/unread:
    get:
      summary: Get team unreads for a user
      description: |-
        Get the count for unread messages and mentions in the teams the user is a member of.
        ##### Permissions
        Must be logged in.
      operationId: get-the-count-for-unread-messages-and-mentions-in-the-teams-the-user-is-a-member-of-permissionsmust-
      x-api-path-slug: usersuser-idteamsunread-get
      parameters:
      - in: query
        name: exclude_team
        description: Optional team id to be excluded from the results
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Unreadsa
      - User
  /users/{user_id}/teams/{team_id}/unread:
    get:
      summary: Get unreads for a team
      description: |-
        Get the unread mention and message counts for a team for the specified user.
        ##### Permissions
        Must be the user or have `edit_other_users` permission and have `view_team` permission for the team.
      operationId: get-the-unread-mention-and-message-counts-for-a-team-for-the-specified-user-permissionsmust-be-the-u
      x-api-path-slug: usersuser-idteamsteam-idunread-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Unreadsa
      - Team
  /teams/{team_id}/invite/email:
    post:
      summary: Invite users to the team by email
      description: |-
        Invite users to the existing team usign the user's email.
        ##### Permissions
        Must have `invite_to_team` permission for the team.
      operationId: invite-users-to-the-existing-team-usign-the-users-email-permissionsmust-have-invite-to-team-permissi
      x-api-path-slug: teamsteam-idinviteemail-post
      parameters:
      - in: body
        name: body
        description: List of users email
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Users
      - To
      - Team
      - By
      - Email
  /teams/{team_id}/import:
    post:
      summary: Import a Team from other application
      description: |-
        Import a team into a existing team. Import users, channels, posts, hooks.
        ##### Permissions
        Must have `permission_import_team` permission.
      operationId: import-a-team-into-a-existing-team-import-users-channels-posts-hooks-permissionsmust-have-permission
      x-api-path-slug: teamsteam-idimport-post
      parameters:
      - in: formData
        name: file
        description: A file to be uploaded in zip format
      - in: formData
        name: filesize
        description: The size of the zip file to be imported
      - in: formData
        name: importFrom
        description: String that defines from which application the team was exported
          to be imported into Mattermost
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Import
      - Team
      - From
      - Other
      - Application
  /teams/invite/{invite_id}:
    get:
      summary: Get invite info for a team
      description: |-
        Get the `name`, `display_name`, `description` and `id` for a team from the invite id.

        __Minimum server version__: 4.0

        ##### Permissions
        No authentication required.
      operationId: get-the-name-display-name-description-and-id-for-a-team-from-the-invite-id-minimum-server-version--4
      x-api-path-slug: teamsinviteinvite-id-get
      parameters:
      - in: path
        name: invite_id
        description: Invite id for a team
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Infoa
      - Team
  /teams/name/{team_name}/channels/name/{channel_name}:
    get:
      summary: Get a channel by name and team name
      description: |-
        Gets a channel from the provided team name and channel name strings.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: gets-a-channel-from-the-provided-team-name-and-channel-name-strings-permissionsread-channel-permissi
      x-api-path-slug: teamsnameteam-namechannelsnamechannel-name-get
      parameters:
      - in: path
        name: channel_name
        description: Channel Name
      - in: path
        name: team_name
        description: Team Name
      responses:
        200:
          description: OK
      tags:
      - Channel
      - By
      - Name
      - Team
      - Name
  /commands:
    get:
      summary: List commands for a team
      description: |-
        List commands for a team.
        ##### Permissions
        `manage_slash_commands` if need list custom commands.
      operationId: list-commands-for-a-team-permissionsmanage-slash-commands-if-need-list-custom-commands
      x-api-path-slug: commands-get
      parameters:
      - in: query
        name: custom_only
        description: To get only the custom commands
      - in: query
        name: team_id
        description: The team id
      responses:
        200:
          description: OK
      tags:
      - List
      - Commandsa
      - Team
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