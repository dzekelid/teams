---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: 'Entertainment Express '
  description: Gets list of teams in a league.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TvMedia/leagues/{LeagueID}/teams:
    get:
      summary: ""
      description: Gets list of teams in a league.
      operationId: GetTvMediaTeams
      x-api-path-slug: tvmedialeaguesleagueidteams-get
      parameters:
      - in: path
        name: LeagueID
        description: League ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Leagues
      - LeagueID
      - Teams
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