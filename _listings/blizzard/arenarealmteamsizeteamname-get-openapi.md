---
swagger: "2.0"
x-collection-name: Blizzard
x-complete: 0
info:
  title: World of Warcraft Get Arena Realm Teamsize Teamname
  description: Provides detailed arena team information.
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