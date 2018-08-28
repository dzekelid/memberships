---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Sets members Active/Inactive system status
  version: 1.0.0
  description: Sets members active/inactive system status.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/branch/{id}/members:
    get:
      summary: Get Branch members by its id.
      description: Get branch members by its id..
      operationId: Branch_MembersByid
      x-api-path-slug: apibranchidmembers-get
      parameters:
      - in: path
        name: id
        description: The id of the Branch members to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Branch
      - Members
      - By
      - Its
      - Id
  /api/group/{id}/setgroupmemberstatus:
    put:
      summary: Sets members Active/Inactive system status
      description: Sets members active/inactive system status.
      operationId: Group_SetGroupMemberStatusByidBygroupMemberStatusDataContract
      x-api-path-slug: apigroupidsetgroupmemberstatus-put
      parameters:
      - in: body
        name: groupMemberStatusDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Members
      - Active
      - Inactive
      - System
      - Status
  /api/role/{id}/vendors:
    get:
      summary: Get the members of a role by the role Id
      description: Get the members of a role by the role id.
      operationId: Role_VendorsByid
      x-api-path-slug: apiroleidvendors-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get the owner information for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Members
      - Of
      - Role
      - By
      - Role
      - Id
  /api/teams/{id}/members:
    get:
      summary: Gets the members of a team
      description: Gets the members of a team.
      operationId: Teams_MembersByid
      x-api-path-slug: apiteamsidmembers-get
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Members
      - Of
      - Team
  /api/teams/{id}/members/add:
    post:
      summary: Adds a member to a team
      description: Adds a member to a team.
      operationId: Teams_AddMemberByidByteamMemberCommands
      x-api-path-slug: apiteamsidmembersadd-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: teamMemberCommands
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Member
      - To
      - Team
  /api/teams/{id}/members/remove:
    post:
      summary: Remove a member from a team
      description: Remove a member from a team.
      operationId: Teams_RemoveMemberByidByremoveTeamMemberCommand
      x-api-path-slug: apiteamsidmembersremove-post
      parameters:
      - in: path
        name: id
        description: Team Id
      - in: body
        name: removeTeamMemberCommand
        description: Details of team members
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Member
      - From
      - Team
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