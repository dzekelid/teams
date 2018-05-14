---
name: Bitbucket
description: Code against the Bitbucket API to automate simple tasks, embed Bitbucket
  data into your own site, build mobile or desktop apps, or even add custom UI add-ons
  into Bitbucket itself using the Connect framework.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bitbucket-logo.png
x-kinRank: "8"
x-alexaRank: ""
tags:
- Stack Network
- Imports
- Developers
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/apis.yaml
specificationVersion: "0.14"
apis:
- name: Bitbucket
  description: Code against the Bitbucket API to automate simple tasks, embed Bitbucket
    data into your own site, build mobile or desktop apps, or even add custom UI add-ons
    into Bitbucket itself using the Connect framework
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bitbucket-logo.png
  humanURL: ""
  baseURL: https://api.bitbucket.org//2.0
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-username-repositories-parameters.md
- name: Bitbucket Add Teams Owner Projects
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bitbucket-logo.png
  humanURL: https://bitbucket.org/
  baseURL: https://api.bitbucket.org//2.0
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/bitbucket/teams-owner-projects-post.md
x-common:
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
  url: https://bitbucket.org/
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
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---