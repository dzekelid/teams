---
name: PagerDuty
x-slug: pagerduty
description: See how PagerDuty Digital Operations Management Platform integrates machine
  data & human intelligence to improve visibility & agility across organizations.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
x-kinRank: "8"
x-alexaRank: "18918"
tags: Teams
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/apis.md
specificationVersion: "0.14"
apis:
- name: PagerDuty Create a team
  x-api-slug: pagerduty
  description: Create a new team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https://///teams
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/teams-post-openapi.md
- name: PagerDuty List teams
  x-api-slug: pagerduty
  description: List teams of your PagerDuty account, optionally filtered by a search
    query.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https://///teams
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/teams-get-openapi.md
- name: PagerDuty Get a team
  x-api-slug: pagerduty
  description: Get details about an existing team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https://///teams/{id}
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/teamsid-get-openapi.md
- name: PagerDuty Delete a team
  x-api-slug: pagerduty
  description: Remove an existing team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https://///teams/{id}
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/teamsid-delete-openapi.md
- name: PagerDuty Update a team
  x-api-slug: pagerduty
  description: Update an existing team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https://///teams/{id}
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/teamsid-put-openapi.md
- name: PagerDuty
  x-api-slug: pagerduty
  description: See how PagerDuty Digital Operations Management Platform integrates
    machine data & human intelligence to improve visibility & agility across organizations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/632-pagerduty.jpg
  humanURL: http://www.pagerduty.com/
  baseURL: https:///
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/pagerduty/openapi.md
x-common:
- type: x-website
  url: http://www.pagerduty.com/
- type: x-base
  url: https://acme.pagerduty.com/api/
- type: x-blog
  url: http://blog.pagerduty.com/
- type: x-blog-rss
  url: http://blog.pagerduty.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/pagerduty
- type: x-crunchbase
  url: https://crunchbase.com/organization/pagerduty
- type: x-developer
  url: http://developer.pagerduty.com/
- type: x-email
  url: info@pagerduty.com
- type: x-email
  url: sales@pagerduty.com
- type: x-email
  url: support@pagerduty.com
- type: x-email
  url: legal@pagerduty.com
- type: x-email
  url: privacy@pagerduty.com
- type: x-github
  url: https://github.com/PagerDuty
- type: x-linkedin
  url: https://www.linkedin.com/company/pagerduty
- type: x-openapi-spec--authoritative
  url: https://api-reference.pagerduty.com/output.json
- type: x-pricing
  url: https://www.pagerduty.com/pricing/
- type: x-twitter
  url: https://twitter.com/pagerduty
- type: x-website
  url: http://www.pagerduty.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---