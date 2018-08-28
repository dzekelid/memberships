swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /memberships:
    delete:
      summary: Delete Memberships
      description: Delete a membership. It requires the **administrator** or **project
        creator** global role or the **project owner** role on the project.
      operationId: DeleteMember
      x-api-path-slug: memberships-delete
      parameters:
      - in: body
        name: membership
        description: Delete membership
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Memberships
    get:
      summary: Get Memberships
      description: |-
        Returns memberships. Supports filtering by projectUri, userUri, userGroupUri, roleUri (but only
        individual values, not multiple) in 'query'.

        If projectURI and userUri/userGroupUri are given a different
        backend path will be used that should be authorized to a project owner even if they wouldn't ordinarily
        be able to see other users' roles.

        It requires the **administrator** or **project creator** global role or the **project owner** role on the project.
        **project owner** requires **projectUri** to be supplied.
      operationId: FindMembers
      x-api-path-slug: memberships-get
      parameters:
      - in: query
        name: query
        description: URI query to prune memberships by
      responses:
        200:
          description: OK
      tags:
      - Memberships
    post:
      summary: Post Memberships
      description: Creates a new membership. It requires the **administrator** or
        **project creator** global role or **project owner** role on the project.
      operationId: CreateMember
      x-api-path-slug: memberships-post
      parameters:
      - in: body
        name: membership
        description: Add new membership
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Memberships
  /membership-roles:
    get:
      summary: Get Membership Roles
      description: Returns membership (project-specific) roles.
      operationId: ListMembershipRoles
      x-api-path-slug: membershiproles-get
      responses:
        200:
          description: OK
      tags:
      - Membership
      - Roles