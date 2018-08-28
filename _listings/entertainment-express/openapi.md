swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
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
  /TvMedia/teams/{TeamID}:
    get:
      summary: ""
      description: Gets details for a specific team.
      operationId: GetTvMediaTeamById
      x-api-path-slug: tvmediateamsteamid-get
      parameters:
      - in: path
        name: TeamID
        description: Team ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Teams
      - TeamID
  /TvMedia/teams/{TeamID}/listings:
    get:
      summary: ""
      description: Retrieve listings for a given TeamID.
      operationId: GetTvMediaTeamListings
      x-api-path-slug: tvmediateamsteamidlistings-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: query
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: path
        name: TeamID
        description: Team ID
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Teams
      - TeamID
      - Listings