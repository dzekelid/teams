---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Teams
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Teams
  x-api-slug: bitbucket
  description: |-
    Returns all the teams that the authenticated user is associated
    with.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams
  tags: Teams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-get-openapi.md
- name: Bitbucket Parameters Teams
  x-api-slug: bitbucket
  description: Parameters teams
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams
  tags: Teams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-parameters-openapi.md
- name: Bitbucket Get Teams Owner Projects
  x-api-slug: bitbucket
  description: Get teams owner projects
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/
  tags: Teams, Owner, Projects
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojects-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojects-get-openapi.md
- name: Bitbucket Parameters Teams Owner Projects
  x-api-slug: bitbucket
  description: Parameters teams owner projects
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/
  tags: Teams, Owner, Projects
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojects-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojects-parameters-openapi.md
- name: Bitbucket Add Teams Owner Projects
  x-api-slug: bitbucket
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/
  tags: Teams, Owner, Projects
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojects-post-openapi.md
- name: Bitbucket Delete Teams Owner Projects Project Key
  x-api-slug: bitbucket
  description: Delete teams owner projects project key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/{project_key}
  tags: Teams, Owner, Projects, Project, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-delete-openapi.md
- name: Bitbucket Get Teams Owner Projects Project Key
  x-api-slug: bitbucket
  description: Get teams owner projects project key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/{project_key}
  tags: Teams, Owner, Projects, Project, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-get-openapi.md
- name: Bitbucket Parameters Teams Owner Projects Project Key
  x-api-slug: bitbucket
  description: Parameters teams owner projects project key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/{project_key}
  tags: Teams, Owner, Projects, Project, Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-parameters-openapi.md
- name: Bitbucket Update Teams Owner Projects Project Key
  x-api-slug: bitbucket
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{owner}/projects/{project_key}
  tags: Teams, Owner, Projects, Project, Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsownerprojectsproject-key-put-openapi.md
- name: Bitbucket Get Teams Username
  x-api-slug: bitbucket
  description: |-
    Gets the public information associated with a team.

    If the team's profile is private, `location`, `website` and
    `created_on` elements are omitted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}
  tags: Teams, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusername-get-openapi.md
- name: Bitbucket Parameters Teams Username
  x-api-slug: bitbucket
  description: Parameters teams username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}
  tags: Teams, Username
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusername-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusername-parameters-openapi.md
- name: Bitbucket Get Teams Username Followers
  x-api-slug: bitbucket
  description: Returns the list of accounts that are following this team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/followers
  tags: Teams, Username, Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowers-get-openapi.md
- name: Bitbucket Parameters Teams Username Followers
  x-api-slug: bitbucket
  description: Parameters teams username followers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/followers
  tags: Teams, Username, Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowers-parameters-openapi.md
- name: Bitbucket Get Teams Username Following
  x-api-slug: bitbucket
  description: Returns the list of accounts this team is following.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/following
  tags: Teams, Username, Following
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowing-get-openapi.md
- name: Bitbucket Parameters Teams Username Following
  x-api-slug: bitbucket
  description: Parameters teams username following
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/following
  tags: Teams, Username, Following
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowing-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamefollowing-parameters-openapi.md
- name: Bitbucket Get Teams Username Hooks
  x-api-slug: bitbucket
  description: Returns a paginated list of webhooks installed on this team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks
  tags: Teams, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-get-openapi.md
- name: Bitbucket Parameters Teams Username Hooks
  x-api-slug: bitbucket
  description: Parameters teams username hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks
  tags: Teams, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-parameters-openapi.md
- name: Bitbucket Add Teams Username Hooks
  x-api-slug: bitbucket
  description: |-
    Creates a new webhook on the specified team.

    Team webhooks are fired for events from all repositories belonging to
    that team account.

    Note that only admins can install webhooks on teams.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks
  tags: Teams, Username, Hooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooks-post-openapi.md
- name: Bitbucket Delete Teams Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Deletes the specified webhook subscription from the given team
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks/{uid}
  tags: Teams, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-delete-openapi.md
- name: Bitbucket Get Teams Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Returns the webhook with the specified id installed on the given
    team account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks/{uid}
  tags: Teams, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-get-openapi.md
- name: Bitbucket Parameters Teams Username Hooks U
  x-api-slug: bitbucket
  description: Parameters teams username hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks/{uid}
  tags: Teams, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-parameters-openapi.md
- name: Bitbucket Update Teams Username Hooks U
  x-api-slug: bitbucket
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/hooks/{uid}
  tags: Teams, Username, Hooks, U
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamehooksuid-put-openapi.md
- name: Bitbucket Get Teams Username Members
  x-api-slug: bitbucket
  description: |-
    All members of a team.

    Returns all members of the specified team. Any member of any of the
    team's groups is considered a member of the team. This includes users
    in groups that may not actually have access to any of the team's
    repositories.

    Note that members using the "private profile" feature are not included.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/members
  tags: Teams, Username, Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamemembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamemembers-get-openapi.md
- name: Bitbucket Parameters Teams Username Members
  x-api-slug: bitbucket
  description: Parameters teams username members
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/members
  tags: Teams, Username, Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamemembers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamemembers-parameters-openapi.md
- name: Bitbucket Get Teams Username Pipelines Config Variables
  x-api-slug: bitbucket
  description: Get teams username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/pipelines_config/variables/
  tags: Teams, Username, Pipelines, Config, Variables
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariables-get-openapi.md
- name: Bitbucket Add Teams Username Pipelines Config Variables
  x-api-slug: bitbucket
  description: Post teams username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/pipelines_config/variables/
  tags: Teams, Username, Pipelines, Config, Variables
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariables-post-openapi.md
- name: Bitbucket Delete Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Delete teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/pipelines_config/variables/{variable_uuid}
  tags: Teams, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket Get Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Get teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/pipelines_config/variables/{variable_uuid}
  tags: Teams, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket Update Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: bitbucket
  description: Put teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/pipelines_config/variables/{variable_uuid}
  tags: Teams, Username, Pipelines, Config, Variables, Variable, Uu
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket Get Teams Username Repositories
  x-api-slug: bitbucket
  description: |-
    All repositories owned by a user/team. This includes private
    repositories, but filtered down to the ones that the calling user has
    access to.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/repositories
  tags: Teams, Username, Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamerepositories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamerepositories-get-openapi.md
- name: Bitbucket Parameters Teams Username Repositories
  x-api-slug: bitbucket
  description: Parameters teams username repositories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//teams/{username}/repositories
  tags: Teams, Username, Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamerepositories-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teamsusernamerepositories-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---