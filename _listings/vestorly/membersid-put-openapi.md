---
swagger: "2.0"
x-collection-name: Vestorly
x-complete: 0
info:
  title: Vestorly Put Members
  description: Updates a single member
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members:
    get:
      summary: Get Members
      description: Returns all members
      operationId: findMembers
      x-api-path-slug: members-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: limit
        description: Number of members to return
      - in: query
        name: start
        description: Skips number of members from start
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
    post:
      summary: Post Members
      description: Create a new member in the Vestorly Platform
      operationId: createMember
      x-api-path-slug: members-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: member
        description: Member you want to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
  /members/{id}:
    get:
      summary: Get Members
      description: Returns a single member
      operationId: findMemberByID
      x-api-path-slug: membersid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of member to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
    put:
      summary: Put Members
      description: Updates a single member
      operationId: updateMemberByID
      x-api-path-slug: membersid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of member to fetch
      - in: body
        name: member
        description: Member you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
  /member_events:
    get:
      summary: Get Member Events
      description: Returns all MemberEvents
      operationId: findMemberEvents
      x-api-path-slug: member-events-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Member
      - Events
  /member_reports:
    get:
      summary: Get Member Reports
      description: Returns all member reports
      operationId: findMemberReports
      x-api-path-slug: member-reports-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Member
      - Reports
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