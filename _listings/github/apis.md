---
name: GitHub
x-slug: github
description: With a community of more than 10 million people, developers can discover,
  use and contribute to over 24 million projects using a powerful, collaborative workflow.    Whether
  using GitHub.com or your own instance of GitHub Enterprise, you can integrate ...
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "70"
tags: Teams
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: Github Get Orgs Org Teams
  x-api-slug: github
  description: List teams.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////orgs/{org}/teams
  tags: Orgs, Org, Teams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/orgsorgteams-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/orgsorgteams-get-openapi.md
- name: Github Add Orgs Org Teams
  x-api-slug: github
  description: |-
    Create team.
    In order to create a team, the authenticated user must be an owner of organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////orgs/{org}/teams
  tags: Orgs, Org, Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/orgsorgteams-post-openapi.md
- name: Github Get Repos Owner Repo Teams
  x-api-slug: github
  description: Get list of teams
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////repos/{owner}/{repo}/teams
  tags: Repos, Owner, Repo, Teams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/reposownerrepoteams-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/reposownerrepoteams-get-openapi.md
- name: Github Delete Teams Team
  x-api-slug: github
  description: |-
    Delete team.
    In order to delete a team, the authenticated user must be an owner of the
    org that the team is associated with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}
  tags: Teams, Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamid-delete-openapi.md
- name: Github Get Teams Team
  x-api-slug: github
  description: Get team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}
  tags: Teams, Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamid-get-openapi.md
- name: Github Patch Teams Team
  x-api-slug: github
  description: |-
    Edit team.
    In order to edit a team, the authenticated user must be an owner of the org
    that the team is associated with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}
  tags: Teams, Team
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamid-patch-openapi.md
- name: Github Get Teams Team Members
  x-api-slug: github
  description: |-
    List team members.
    In order to list members in a team, the authenticated user must be a member
    of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/members
  tags: Teams, Team, Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembers-get-openapi.md
- name: Github Delete Teams Team Members Username
  x-api-slug: github
  description: |-
    The "Remove team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Remove team membership API instead. It allows you to remove both active and pending memberships.

    Remove team member.
    In order to remove a user from a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
    NOTE This does not delete the user, it just remove them from the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/members/{username}
  tags: Teams, Team, Members, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-delete-openapi.md
- name: Github Get Teams Team Members Username
  x-api-slug: github
  description: |-
    The "Get team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Get team membership API instead. It allows you to get both active and pending memberships.

    Get team member.
    In order to get if a user is a member of a team, the authenticated user mus
    be a member of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/members/{username}
  tags: Teams, Team, Members, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-get-openapi.md
- name: Github Put Teams Team Members Username
  x-api-slug: github
  description: |-
    The API (described below) is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Add team membership API instead. It allows you to invite new organization members to your teams.

    Add team member.
    In order to add a user to a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/members/{username}
  tags: Teams, Team, Members, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembersusername-put-openapi.md
- name: Github Delete Teams Team Memberships Username
  x-api-slug: github
  description: |-
    Remove team membership.
    In order to remove a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with. NOTE: This does not delete the user, it just removes their membership from the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/memberships/{username}
  tags: Teams, Team, Memberships, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-delete-openapi.md
- name: Github Get Teams Team Memberships Username
  x-api-slug: github
  description: |-
    Get team membership.
    In order to get a user's membership with a team, the authenticated user must be a member of the team or an owner of the team's organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/memberships/{username}
  tags: Teams, Team, Memberships, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-get-openapi.md
- name: Github Put Teams Team Memberships Username
  x-api-slug: github
  description: |-
    Add team membership.
    In order to add a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with.

    If the user is already a part of the team's organization (meaning they're on at least one other team in the organization), this endpoint will add the user to the team.

    If the user is completely unaffiliated with the team's organization (meaning they're on none of the organization's teams), this endpoint will send an invitation to the user via email. This newly-created membership will be in the 'pending' state until the user accepts the invitation, at which point the membership will transition to the 'active' state and the user will be added as a member of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/memberships/{username}
  tags: Teams, Team, Memberships, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidmembershipsusername-put-openapi.md
- name: Github Get Teams Team Repos
  x-api-slug: github
  description: List team repos
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/repos
  tags: Teams, Team, Repos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidrepos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidrepos-get-openapi.md
- name: Github Put Teams Team Repos Org Repo
  x-api-slug: github
  description: In order to add a repository to a team, the authenticated user must
    be an owner of the org that the team is associated with. Also, the repository
    must be owned by the organization, or a direct fork of a repository owned by the
    organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/repos/{org}/{repo}
  tags: Teams, Team, Repos, Org, Repo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposorgrepo-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposorgrepo-put-openapi.md
- name: Github Delete Teams Team Repos Owner Repo
  x-api-slug: github
  description: 'In order to remove a repository from a team, the authenticated user
    must be an owner of the org that the team is associated with. NOTE: This does
    not delete the repository, it just removes it from the team.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/repos/{owner}/{repo}
  tags: Teams, Team, Repos, Owner, Repo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposownerrepo-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposownerrepo-delete-openapi.md
- name: Github Get Teams Team Repos Owner Repo
  x-api-slug: github
  description: Check if a team manages a repository
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////teams/{teamId}/repos/{owner}/{repo}
  tags: Teams, Team, Repos, Owner, Repo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposownerrepo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/teamsteamidreposownerrepo-get-openapi.md
- name: Github Get User Teams
  x-api-slug: github
  description: List all of the teams across all of the organizations to which the
    authenticated user belongs. This method requires user or repo scope when authenticating
    via OAuth.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com////user/teams
  tags: User, Teams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/userteams-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/userteams-get-openapi.md
- name: Github
  x-api-slug: github
  description: With a community of more than 10 million people, developers can discover,
    use and contribute to over 24 million projects using a powerful, collaborative
    workflow.    Whether using GitHub.com or your own instance of GitHub Enterprise,
    you can integrate ...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/github/openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---