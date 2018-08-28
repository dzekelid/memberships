---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Organizations Memberships
  description: Get organizations memberships.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/memberships:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoard
      x-api-path-slug: boardsidboardmemberships-get
      parameters:
      - in: query
        name: filter
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /boards/{idBoard}/memberships/{idMembership}:
    get:
      summary: Get Boards Memberships
      description: Get boards memberships.
      operationId: getBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
    put:
      summary: Put Boards Memberships
      description: Put boards memberships.
      operationId: updateBoardsMembershipsByIdBoardByIdMembership
      x-api-path-slug: boardsidboardmembershipsidmembership-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Memberships to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMembership
        description: idMembership
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Memberships
  /organizations/{idOrg}/memberships:
    get:
      summary: Get Organizations Memberships
      description: Get organizations memberships.
      operationId: getOrganizationsMembershipsByIdOrg
      x-api-path-slug: organizationsidorgmemberships-get
      parameters:
      - in: query
        name: filter
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: member
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
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