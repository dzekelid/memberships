---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: WebEx Teams API Get membership details
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
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
    post:
      summary: Create a membership
      description: |-
        Add someone to a room by Person ID or email address; optionally making them a moderator.

        https://developer.webex.com/endpoint-memberships-post.html
      operationId: MembershipsPost
      x-api-path-slug: memberships-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
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
    post:
      summary: Create a team membership
      description: |-
        Add someone to a team by Person ID or email address; optionally making them a moderator.

        https://developer.webex.com/endpoint-teammemberships-post.html
      operationId: TeamMembershipsPost
      x-api-path-slug: teammemberships-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
  /memberships/{_membership}:
    get:
      summary: Get membership details
      description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
        ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
      operationId: MembershipsByMembershipGet
      x-api-path-slug: memberships-membership-get
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
      - Details
    put:
      summary: Update a membership
      description: |-
        Updates properties for a membership by ID.

        Specify the membership ID in the membershipId URI parameter.

        https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
      operationId: MembershipsByMembershipPut
      x-api-path-slug: memberships-membership-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
    delete:
      summary: Delete membership
      description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in
        the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
      operationId: MembershipsByMembershipDelete
      x-api-path-slug: memberships-membership-delete
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
  /team/memberships/{_membership}:
    get:
      summary: Get team membership details
      description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
        ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
      operationId: TeamMembershipsByMembershipGet
      x-api-path-slug: teammemberships-membership-get
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
      - Details
    put:
      summary: Update a team membership
      description: |-
        Updates properties for a membership by ID.

        Specify the membership ID in the membershipId URI parameter.

        https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
      operationId: TeamMembershipsByMembershipPut
      x-api-path-slug: teammemberships-membership-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
    delete:
      summary: Delete a team membership
      description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in
        the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
      operationId: TeamMembershipsByMembershipDelete
      x-api-path-slug: teammemberships-membership-delete
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
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