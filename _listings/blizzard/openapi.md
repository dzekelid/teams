---
swagger: "2.0"
x-collection-name: Blizzard
x-complete: 1
info:
  title: World of Warcraft
  description: welcome-to-the-restful-apis-exposed-through-the-world-of-warcraft-community-site-as-a-service-to-the-world-of-warcraft-community-
  version: 1.0.0
host: us.battle.net
basePath: /api/wow/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /arena/{realm}/{teamSize}/{teamName}:
    get:
      summary: Get Arena Realm Teamsize Teamname
      description: Provides detailed arena team information.
      operationId: getArenaRealmTeamsizeTeamname
      x-api-path-slug: arenarealmteamsizeteamname-get
      parameters:
      - in: path
        name: realm
        description: The realm name
      - in: path
        name: teamName
        description: The team name
      - in: path
        name: teamSize
        description: The team size
      responses:
        200:
          description: OK
      tags:
      - Arena
      - Realm
      - TeamSize
      - TeamName
---