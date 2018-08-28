swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/memberships:
    get:
      summary: Get Account Memberships
      description: ID of a user should be specified as a query parameter. JSON with
        membership details is returned. For this API call system/admin or system/manager
        role is required
      operationId: getMembershipsOfSpecificUser
      x-api-path-slug: accountmemberships-get
      parameters:
      - in: query
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Memberships
  /account/{id}/members:
    get:
      summary: Get Account Members
      description: Get all members for a specific account. This API call requires
        account/owner, system/admin or system/manager role.
      operationId: getMembers
      x-api-path-slug: accountidmembers-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
    post:
      summary: Post Account Members
      description: Add a new user to an account. This user will have account/member
        role. This API call requires account/owner, system/admin or system/manager
        role.
      operationId: addMember
      x-api-path-slug: accountidmembers-post
      parameters:
      - in: body
        name: body
        description: New membership
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
  /account/{id}/members/{userid}:
    delete:
      summary: Delete Account Members User
      description: Remove user from a specific account. This API call requires account/owner,
        system/admin or system/manager role.
      operationId: removeMember
      x-api-path-slug: accountidmembersuserid-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Members
      - Userid