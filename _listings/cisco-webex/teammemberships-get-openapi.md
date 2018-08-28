---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: WebEx Teams API List team memberships
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /memberships:
    get:
      summary: List memberships (for all rooms)
      description: |-
        Lists all room memberships. By default, lists memberships for rooms to which the authenticated user belongs.

        Use query parameters to filter the response.

        Use roomId to list memberships for a room, by ID.

        Use either personId or personEmail to filter the results.

        https://developer.webex.com/endpoint-memberships-get.html
      operationId: MembershipsGet2
      x-api-path-slug: memberships-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Memberships
      - (for
      - ""
      - Rooms)
  /team/memberships:
    get:
      summary: List team memberships
      description: "Lists all team memberships. By default, lists memberships for
        teams to which the authenticated user belongs.\r\n\r\nUse query parameters
        to filter the response.\r\n\r\nUse teamId to list memberships for a team,
        by ID.\r\n\r\nUse either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
      operationId: TeamMembershipsGet
      x-api-path-slug: teammemberships-get
      parameters:
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Team
      - Memberships
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