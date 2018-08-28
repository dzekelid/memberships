---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Put Groups Group Members Member
  description: |-
    ### Delete a Group Member
    Updates a member with the ```member_id``` to the group with a ```group_id```.
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/members:
    get:
      summary: Get Groups Group Members
      description: |-
        ### List all Group Members
        Page through a list of all members of a group with a ```group_id```. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-group-memberspage-through-a-list-of-all-members-of-a-group-with-a-group-id-you-can-specify
      x-api-path-slug: groupsgroup-idmembers-get
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
    post:
      summary: Post Groups Group Members
      description: |-
        ### Create a Group Member

        Adds a member to a group with a ```group_id```. ???Make sure you provide an accurate email address and/or phone number or alerts will not be received by the member.
      operationId: -create-a-group-memberadds-a-member-to-a-group-with-a-group-id-make-sure-you-provide-an-accurate-ema
      x-api-path-slug: groupsgroup-idmembers-post
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_id
        description: UUID of the Group
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
  /groups/{group_id}/members/{member_id}:
    put:
      summary: Put Groups Group Members Member
      description: |-
        ### Delete a Group Member
        Updates a member with the ```member_id``` to the group with a ```group_id```.
      operationId: -delete-a-group-memberupdates-a-member-with-the-member-id-to-the-group-with-a-group-id
      x-api-path-slug: groupsgroup-idmembersmember-id-put
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_id
        description: UUID of the Group
      - in: path
        name: member_id
        description: UUID of the User
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
      - Member
    delete:
      summary: Delete Groups Group Members Member
      description: |-
        ### Delete a Group Member
        Removes a member with the ```member_id``` from the group with a ```group_id```.
      operationId: -delete-a-group-memberremoves-a-member-with-the-member-id-from-the-group-with-a-group-id
      x-api-path-slug: groupsgroup-idmembersmember-id-delete
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      - in: path
        name: member_id
        description: UUID of the User
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
      - Member
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