---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Teams
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Get teams
  x-api-slug: teams-get
  description: |-
    For regular users only returns open teams. Users with the "manage_system" permission will return teams regardless of type. The result is based on query string parameters - page and per_page.
    ##### Permissions
    Must be authenticated. "manage_system" permission is required to show all teams.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teams-get-openapi.md
- name: Mattermost API Reference - Search teams
  x-api-slug: teamssearch-post
  description: |-
    Search teams based on search term provided in the request body.
    ##### Permissions
    Logged in user only shows open teams
    Logged in user with "manage_system" permission shows all teams
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamssearch-post-openapi.md
- name: Mattermost API Reference - Get a user's teams
  x-api-slug: usersuser-idteams-get
  description: |-
    Get a list of teams that a user is on.
    ##### Permissions
    Must be authenticated as the user or have the `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteams-get-openapi.md
- name: Mattermost API Reference - Create a team
  x-api-slug: teams-post
  description: |-
    Create a new team on the system.
    ##### Permissions
    Must be authenticated and have the `create_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teams-post-openapi.md
- name: Mattermost API Reference - Get a team
  x-api-slug: teamsteam-id-get
  description: |-
    Get a team on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-get-openapi.md
- name: Mattermost API Reference - Update a team
  x-api-slug: teamsteam-id-put
  description: |-
    Update a team by providing the team object. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-put-openapi.md
- name: Mattermost API Reference - Delete a team
  x-api-slug: teamsteam-id-delete
  description: |-
    Soft deletes a team, by marking the team as deleted in the database. Soft deleted teams will not be accessible in the user interface.

    Optionally use the permanent query parameter to hard delete the team for compliance reasons.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-delete-openapi.md
- name: Mattermost API Reference - Patch a team
  x-api-slug: teamsteam-idpatch-put
  description: |-
    Partially update a team by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idpatch-put-openapi.md
- name: Mattermost API Reference - Get a team by name
  x-api-slug: teamsnamename-get
  description: |-
    Get a team based on provided name string
    ##### Permissions
    Must be authenticated, team type is open and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnamename-get-openapi.md
- name: Mattermost API Reference - Check if team exists
  x-api-slug: teamsnamenameexists-get
  description: Check if the team exists based on a team name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnamenameexists-get-openapi.md
- name: Mattermost API Reference - Get team members
  x-api-slug: teamsteam-idmembers-get
  description: |-
    Get a page team members list based on query string parameters - team id, page and per page.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembers-get-openapi.md
- name: Mattermost API Reference - Add user to team
  x-api-slug: teamsteam-idmembers-post
  description: |-
    Add user to the team by user_id.
    ##### Permissions
    Must be authenticated and team be open to add self. For adding another user, authenticated user must have the `add_user_to_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembers-post-openapi.md
- name: Mattermost API Reference - Add user to team from invite
  x-api-slug: teamsmembersinvite-post
  description: |-
    Using either an invite id or hash/data pair from an email invite link, add a user to a team.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsmembersinvite-post-openapi.md
- name: Mattermost API Reference - Add multiple users to team
  x-api-slug: teamsteam-idmembersbatch-post
  description: |-
    Add a number of users to the team by user_id.
    ##### Permissions
    Must be authenticated. Authenticated user must have the `add_user_to_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersbatch-post-openapi.md
- name: Mattermost API Reference - Get team members for a user
  x-api-slug: usersuser-idteamsmembers-get
  description: |-
    Get a list of team members for a user. Useful for getting the ids of teams the user is on and the roles they have in those teams.
    ##### Permissions
    Must be logged in as the user or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsmembers-get-openapi.md
- name: Mattermost API Reference - Get a team member
  x-api-slug: teamsteam-idmembersuser-id-get
  description: |-
    Get a team member on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Remove user from team
  x-api-slug: teamsteam-idmembersuser-id-delete
  description: |-
    Delete the team member object for a user, effectively removing them from a team.
    ##### Permissions
    Must be logged in as the user or have the `remove_user_from_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Get team members by ids
  x-api-slug: teamsteam-idmembersids-post
  description: |-
    Get a list of team members based on a provided array of user ids.
    ##### Permissions
    Must have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get a team stats
  x-api-slug: teamsteam-idstats-get
  description: |-
    Get a team stats on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idstats-get-openapi.md
- name: Mattermost API Reference - Get the team icon
  x-api-slug: teamsteam-idimage-get
  description: |-
    Get the team icon of the team.

    __Minimum server version__: 4.9

    ##### Permissions
    User must be authenticated. In addition, team must be open or the user must have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimage-get-openapi.md
- name: Mattermost API Reference - Sets the team icon
  x-api-slug: teamsteam-idimage-post
  description: |-
    Sets the team icon for the team.

    __Minimum server version__: 4.9

    ##### Permissions
    Must be authenticated and have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimage-post-openapi.md
- name: Mattermost API Reference - Update a team member roles
  x-api-slug: teamsteam-idmembersuser-idroles-put
  description: |-
    Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
    ##### Permissions
    Must be authenticated and have the `manage_team_roles` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Get team unreads for a user
  x-api-slug: usersuser-idteamsunread-get
  description: |-
    Get the count for unread messages and mentions in the teams the user is a member of.
    ##### Permissions
    Must be logged in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsunread-get-openapi.md
- name: Mattermost API Reference - Get unreads for a team
  x-api-slug: usersuser-idteamsteam-idunread-get
  description: |-
    Get the unread mention and message counts for a team for the specified user.
    ##### Permissions
    Must be the user or have `edit_other_users` permission and have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsteam-idunread-get-openapi.md
- name: Mattermost API Reference - Invite users to the team by email
  x-api-slug: teamsteam-idinviteemail-post
  description: |-
    Invite users to the existing team usign the user's email.
    ##### Permissions
    Must have `invite_to_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idinviteemail-post-openapi.md
- name: Mattermost API Reference - Import a Team from other application
  x-api-slug: teamsteam-idimport-post
  description: |-
    Import a team into a existing team. Import users, channels, posts, hooks.
    ##### Permissions
    Must have `permission_import_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimport-post-openapi.md
- name: Mattermost API Reference - Get invite info for a team
  x-api-slug: teamsinviteinvite-id-get
  description: |-
    Get the `name`, `display_name`, `description` and `id` for a team from the invite id.

    __Minimum server version__: 4.0

    ##### Permissions
    No authentication required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsinviteinvite-id-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - Get a channel by name and team name
  x-api-slug: teamsnameteam-namechannelsnamechannel-name-get
  description: |-
    Gets a channel from the provided team name and channel name strings.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnameteam-namechannelsnamechannel-name-get-openapi.md
- name: Mattermost API Reference - Get invite info for a team
  x-api-slug: teamsinviteinvite-id-get
  description: |-
    Get the `name`, `display_name`, `description` and `id` for a team from the invite id.

    __Minimum server version__: 4.0

    ##### Permissions
    No authentication required.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsinviteinvite-id-get-openapi.md
- name: Mattermost API Reference - Import a Team from other application
  x-api-slug: teamsteam-idimport-post
  description: |-
    Import a team into a existing team. Import users, channels, posts, hooks.
    ##### Permissions
    Must have `permission_import_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimport-post-openapi.md
- name: Mattermost API Reference - Invite users to the team by email
  x-api-slug: teamsteam-idinviteemail-post
  description: |-
    Invite users to the existing team usign the user's email.
    ##### Permissions
    Must have `invite_to_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idinviteemail-post-openapi.md
- name: Mattermost API Reference - Get unreads for a team
  x-api-slug: usersuser-idteamsteam-idunread-get
  description: |-
    Get the unread mention and message counts for a team for the specified user.
    ##### Permissions
    Must be the user or have `edit_other_users` permission and have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsteam-idunread-get-openapi.md
- name: Mattermost API Reference - Get team unreads for a user
  x-api-slug: usersuser-idteamsunread-get
  description: |-
    Get the count for unread messages and mentions in the teams the user is a member of.
    ##### Permissions
    Must be logged in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsunread-get-openapi.md
- name: Mattermost API Reference - Update a team member roles
  x-api-slug: teamsteam-idmembersuser-idroles-put
  description: |-
    Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
    ##### Permissions
    Must be authenticated and have the `manage_team_roles` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Sets the team icon
  x-api-slug: teamsteam-idimage-post
  description: |-
    Sets the team icon for the team.

    __Minimum server version__: 4.9

    ##### Permissions
    Must be authenticated and have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimage-post-openapi.md
- name: Mattermost API Reference - Get the team icon
  x-api-slug: teamsteam-idimage-get
  description: |-
    Get the team icon of the team.

    __Minimum server version__: 4.9

    ##### Permissions
    User must be authenticated. In addition, team must be open or the user must have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idimage-get-openapi.md
- name: Mattermost API Reference - Get a team stats
  x-api-slug: teamsteam-idstats-get
  description: |-
    Get a team stats on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idstats-get-openapi.md
- name: Mattermost API Reference - Get team members by ids
  x-api-slug: teamsteam-idmembersids-post
  description: |-
    Get a list of team members based on a provided array of user ids.
    ##### Permissions
    Must have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersids-post-openapi.md
- name: Mattermost API Reference - Remove user from team
  x-api-slug: teamsteam-idmembersuser-id-delete
  description: |-
    Delete the team member object for a user, effectively removing them from a team.
    ##### Permissions
    Must be logged in as the user or have the `remove_user_from_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-id-delete-openapi.md
- name: Mattermost API Reference - Get a team member
  x-api-slug: teamsteam-idmembersuser-id-get
  description: |-
    Get a team member on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Get team members for a user
  x-api-slug: usersuser-idteamsmembers-get
  description: |-
    Get a list of team members for a user. Useful for getting the ids of teams the user is on and the roles they have in those teams.
    ##### Permissions
    Must be logged in as the user or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/usersuser-idteamsmembers-get-openapi.md
- name: Mattermost API Reference - Add multiple users to team
  x-api-slug: teamsteam-idmembersbatch-post
  description: |-
    Add a number of users to the team by user_id.
    ##### Permissions
    Must be authenticated. Authenticated user must have the `add_user_to_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembersbatch-post-openapi.md
- name: Mattermost API Reference - Add user to team from invite
  x-api-slug: teamsmembersinvite-post
  description: |-
    Using either an invite id or hash/data pair from an email invite link, add a user to a team.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsmembersinvite-post-openapi.md
- name: Mattermost API Reference - Add user to team
  x-api-slug: teamsteam-idmembers-post
  description: |-
    Add user to the team by user_id.
    ##### Permissions
    Must be authenticated and team be open to add self. For adding another user, authenticated user must have the `add_user_to_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembers-post-openapi.md
- name: Mattermost API Reference - Get team members
  x-api-slug: teamsteam-idmembers-get
  description: |-
    Get a page team members list based on query string parameters - team id, page and per page.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idmembers-get-openapi.md
- name: Mattermost API Reference - Check if team exists
  x-api-slug: teamsnamenameexists-get
  description: Check if the team exists based on a team name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnamenameexists-get-openapi.md
- name: Mattermost API Reference - Get a team by name
  x-api-slug: teamsnamename-get
  description: |-
    Get a team based on provided name string
    ##### Permissions
    Must be authenticated, team type is open and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsnamename-get-openapi.md
- name: Mattermost API Reference - Patch a team
  x-api-slug: teamsteam-idpatch-put
  description: |-
    Partially update a team by providing only the fields you want to update. Omitted fields will not be updated. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-idpatch-put-openapi.md
- name: Mattermost API Reference - Delete a team
  x-api-slug: teamsteam-id-delete
  description: |-
    Soft deletes a team, by marking the team as deleted in the database. Soft deleted teams will not be accessible in the user interface.

    Optionally use the permanent query parameter to hard delete the team for compliance reasons.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-delete-openapi.md
- name: Mattermost API Reference - Update a team
  x-api-slug: teamsteam-id-put
  description: |-
    Update a team by providing the team object. The fields that can be updated are defined in the request body, all other provided fields will be ignored.
    ##### Permissions
    Must have the `manage_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-put-openapi.md
- name: Mattermost API Reference - Get a team
  x-api-slug: teamsteam-id-get
  description: |-
    Get a team on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teamsteam-id-get-openapi.md
- name: Mattermost API Reference - Create a team
  x-api-slug: teams-post
  description: |-
    Create a new team on the system.
    ##### Permissions
    Must be authenticated and have the `create_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/mattermost/teams-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---