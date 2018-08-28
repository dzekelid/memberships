---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Organizations Org Membership  Refuse
  description: Refuse user membership to a given organization
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org}/membership/:
    get:
      summary: Get Organizations Org Membership
      description: List membership requests for a given organization
      operationId: getOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-get
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: query
        name: status
        description: If provided, only return requests ith a given status
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
    post:
      summary: Add Organizations Org Membership
      description: Apply for membership to a given organization
      operationId: postOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
  /organizations/{org}/membership/{id}/accept/:
    post:
      summary: Add Organizations Org Membership  Accept
      description: Accept user membership to a given organization
      operationId: postOrganizationsOrgMembershipAccept
      x-api-path-slug: organizationsorgmembershipidaccept-post
      parameters:
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Accept
  /organizations/{org}/membership/{id}/refuse/:
    post:
      summary: Add Organizations Org Membership  Refuse
      description: Refuse user membership to a given organization
      operationId: postOrganizationsOrgMembershipRefuse
      x-api-path-slug: organizationsorgmembershipidrefuse-post
      parameters:
      - in: body
        name: comment
        description: The refusal reason
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Refuse
  /organizations/{org}/member/{user}:
    delete:
      summary: Delete Organizations Org Member User
      description: Delete member from an organization
      operationId: deleteOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-delete
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    post:
      summary: Add Organizations Org Member User
      description: Add a member into a given organization
      operationId: postOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    put:
      summary: Put Organizations Org Member User
      description: Update member status into a given organization
      operationId: putOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-put
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
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