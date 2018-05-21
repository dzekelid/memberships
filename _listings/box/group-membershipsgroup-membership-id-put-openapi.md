---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Update Membership
  description: Used to update a group membership.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /group_memberships:
    post:
      summary: Create Membership
      description: Used to add a member to a Group.
      operationId: createGroupMembership
      x-api-path-slug: group-memberships-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
  /group_memberships/{GROUP_MEMBERSHIP_ID}:
    get:
      summary: Get Membership
      description: Fetches a specific group membership entry.
      operationId: getGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_MEMBERSHIP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
      - Group
      - Membership
    put:
      summary: Update Membership
      description: Used to update a group membership.
      operationId: updateGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_MEMBERSHIP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
      - Group
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