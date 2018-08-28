---
name: Cisco WebEx
x-slug: cisco-webex
description: Cisco Webex is the leading enterprise solution for video conferencing
  & web conferencing today. This secure software-based platform for video & audio
  conferencing, group messaging & webinars helps organizations be more productive.Participants
  can join ...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
x-kinRank: "7"
x-alexaRank: "632"
tags: Teams
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/apis.md
specificationVersion: "0.14"
apis:
- name: Webex Teams API - List teams
  x-api-slug: teams-get
  description: |-
    List teams.

    https://developer.webex.com/endpoint-teams-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-get-openapi.md
- name: Webex Teams API - Create a Team room
  x-api-slug: rooms-post
  description: |-
    Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

    https://developer.webex.com/endpoint-rooms-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-post-openapi.md
- name: Webex Teams API - Get Team room details
  x-api-slug: rooms-room-get
  description: "Shows details for a room, by ID.\r\n\r\nSpecify the room ID in the
    roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-room-get-openapi.md
- name: Webex Teams API - Delete a Team room
  x-api-slug: rooms-room-delete
  description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId parameter
    in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-room-delete-openapi.md
- name: Webex Teams API - Create a team
  x-api-slug: teams-post
  description: |-
    Create a new team.

    https://developer.webex.com/endpoint-teams-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-post-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Get team details
  x-api-slug: teams-team-get
  description: |-
    Show details for a team.

    https://developer.webex.com/endpoint-teams-teamId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-get-openapi.md
- name: Webex Teams API - Update a team
  x-api-slug: teams-team-put
  description: |-
    Update a team.

    https://developer.webex.com/endpoint-teams-teamId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-put-openapi.md
- name: Webex Teams API - Delete a team
  x-api-slug: teams-team-delete
  description: |-
    Delete a team.

    https://developer.webex.com/endpoint-teams-teamId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-delete-openapi.md
- name: Webex Teams API - List team memberships
  x-api-slug: teammemberships-get
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-get-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - List team memberships
  x-api-slug: teammemberships-get
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-get-openapi.md
- name: Webex Teams API - List team memberships
  x-api-slug: teammemberships-get
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-get-openapi.md
- name: Webex Teams API - Delete a team
  x-api-slug: teams-team-delete
  description: |-
    Delete a team.

    https://developer.webex.com/endpoint-teams-teamId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-delete-openapi.md
- name: Webex Teams API - Delete a team
  x-api-slug: teams-team-delete
  description: |-
    Delete a team.

    https://developer.webex.com/endpoint-teams-teamId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-delete-openapi.md
- name: Webex Teams API - Update a team
  x-api-slug: teams-team-put
  description: |-
    Update a team.

    https://developer.webex.com/endpoint-teams-teamId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-put-openapi.md
- name: Webex Teams API - Update a team
  x-api-slug: teams-team-put
  description: |-
    Update a team.

    https://developer.webex.com/endpoint-teams-teamId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-put-openapi.md
- name: Webex Teams API - Get team details
  x-api-slug: teams-team-get
  description: |-
    Show details for a team.

    https://developer.webex.com/endpoint-teams-teamId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-get-openapi.md
- name: Webex Teams API - Get team details
  x-api-slug: teams-team-get
  description: |-
    Show details for a team.

    https://developer.webex.com/endpoint-teams-teamId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-team-get-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Create a team
  x-api-slug: teams-post
  description: |-
    Create a new team.

    https://developer.webex.com/endpoint-teams-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/teams-post-openapi.md
- name: Webex Teams API - Delete a Team room
  x-api-slug: rooms-room-delete
  description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId parameter
    in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-room-delete-openapi.md
- name: Webex Teams API - Delete a Team room
  x-api-slug: rooms-room-delete
  description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId parameter
    in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-room-delete-openapi.md
- name: Webex Teams API - Get Team room details
  x-api-slug: rooms-room-get
  description: "Shows details for a room, by ID.\r\n\r\nSpecify the room ID in the
    roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-room-get-openapi.md
- name: Webex Teams API - Create a Team room
  x-api-slug: rooms-post
  description: |-
    Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

    https://developer.webex.com/endpoint-rooms-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-post-openapi.md
- name: Webex Teams API - Create a Team room
  x-api-slug: rooms-post
  description: |-
    Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

    https://developer.webex.com/endpoint-rooms-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/cisco-webex/rooms-post-openapi.md
x-common:
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/1f5e101d8290a5303c90
- type: x-api-gallery
  url: http://cisco.unity.connection.messaging.interface.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cisco.webex.stack.network
- type: x-blog
  url: http://blogs.webex.com/
- type: x-blog-rss
  url: http://blogs.webex.com/webex_interactions/index.rdf
- type: x-crunchbase
  url: https://crunchbase.com/organization/webex-communications
- type: x-crunchbase
  url: http://www.crunchbase.com/company/webex
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/0aa22af74405f82086d4
- type: x-twitter
  url: https://twitter.com/webex
- type: x-developer
  url: https://developer.webex.com/
- type: x-website
  url: https://webex.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---