---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava List Club Members
  description: Returns a list of the athletes who are members of a given club.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clubs/{id}/members:
    get:
      summary: List Club Members
      description: Returns a list of the athletes who are members of a given club.
      operationId: getClubMembersById
      x-api-path-slug: clubsidmembers-get
      parameters:
      - in: path
        name: id
        description: The identifier of the club
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Club
      - Members
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