---
name: Blizzard
x-slug: blizzard
description: This is the documentation for the RESTful APIs exposed through the World
  of Warcraft community site as a service to the World of Warcraft community.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Blizzard_Entertainment_Logo.svg.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Teams
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/blizzard/apis.md
specificationVersion: "0.14"
apis:
- name: World of Warcraft Get Arena Realm Teamsize Teamname
  x-api-slug: world-of-warcraft
  description: Provides detailed arena team information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Blizzard_Entertainment_Logo.svg.png
  humanURL: http://battle.net
  baseURL: https://us.battle.net//api/wow///arena/{realm}/{teamSize}/{teamName}
  tags: Arena,Realm,TeamSize,TeamName
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/blizzard/arenarealmteamsizeteamname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/blizzard/arenarealmteamsizeteamname-get-openapi.md
- name: World of Warcraft
  x-api-slug: world-of-warcraft
  description: Battle.net is a site that aims to unite all Blizzard gamers under the
    banner of a single, powerful, and advanced online gaming service. Gamers around
    the world meet up on Battle.net to prove their skill in multiplayer matches or
    to socialize with their friends. The World of Warcraft specific APIs are available
    to the Battle.net community, developers and partners to help expose some of the
    sought after data already served by the World of Warcraft community site. Currently
    data exposed includes realm status with  character, guild and arena team profile
    pages information to come later. The API uses RESTful calls and responses are
    formatted in JSON and JSONP.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Blizzard_Entertainment_Logo.svg.png
  humanURL: http://battle.net
  baseURL: https://us.battle.net//api/wow/
  tags: Teams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/teams/master/_listings/blizzard/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/blizzard.json
- type: x-developer
  url: https://dev.battle.net/
- type: x-github
  url: https://github.com/Blizzard
- type: x-twitter
  url: Blizzard_Ent
- type: x-website
  url: http://battle.net
- type: x-website
  url: https://www.blizzard.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---