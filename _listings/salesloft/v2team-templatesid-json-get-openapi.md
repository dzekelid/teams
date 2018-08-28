---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch a team template
  description: Fetches a team template, by ID only.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/team.json:
    get:
      summary: Fetch current team
      description: Fetches the team of the authenticated user.
      operationId: v2.team.json.get
      x-api-path-slug: v2team-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Current
      - Team
  /v2/team_templates.json:
    get:
      summary: List team templates
      description: |-
        Fetches multiple team template records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Team templates are templates that are available team-wide. Admins may use
        team templates to create original content for the entire team, monitor version control to ensure templates are always up to date,
        and track template performance across the entire organization. All metrics on a team template reflect usage across the team; individual metrics can be found with the email_templates API endpoint.
      operationId: v2.team_templates.json.get
      x-api-path-slug: v2team-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of team templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Team
      - Templates
  /v2/team_templates/{id}.json:
    get:
      summary: Fetch a team template
      description: Fetches a team template, by ID only.
      operationId: v2.team_templates.id.json.get
      x-api-path-slug: v2team-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: Team Template ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Team
      - Template
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