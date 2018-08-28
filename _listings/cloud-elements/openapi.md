swagger: "2.0"
x-collection-name: Cloud Elements
x-complete: 1
info:
  title: zohocrm
  version: api-v2
host: console.cloud-elements.com
basePath: /elements/api-v2/hubs/crm
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/get_membership:
    post:
      summary: Get Membership
      description: Get membership.
      operationId: postReportsGetMembership
      x-api-path-slug: reportsget-membership-post
      parameters:
      - in: query
        name: end_date
        description: optional ending date (exclusive)
      - in: query
        name: start_date
        description: optional starting date (inclusive)
      responses:
        200:
          description: OK
      tags:
      - Membership
  /members/list:
    post:
      summary: List Members
      description: List members.
      operationId: postMembersList
      x-api-path-slug: memberslist-post
      parameters:
      - in: query
        name: cursor
        description: optional encoded value indicating from what point to get the
          next limit members
      - in: query
        name: limit
        description: optional number of results to return per call (default 1000,
          maximum 1000)
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  /members/add:
    post:
      summary: Add Member
      description: Add member.
      operationId: postMembersAdd
      x-api-path-slug: membersadd-post
      parameters:
      - in: query
        name: member_email
        description: member email
      - in: query
        name: member_external_id
        description: optional external ID for member
      - in: query
        name: member_given_name
        description: member first name
      - in: query
        name: member_surname
        description: member last name
      - in: query
        name: send_welcome_email
        description: optional boolean to send a welcome email to the member
      responses:
        200:
          description: OK
      tags:
      - Member
  /members/get_info:
    post:
      summary: Get Member Info
      description: Get member info.
      operationId: postMembersGetInfo
      x-api-path-slug: membersget-info-post
      parameters:
      - in: query
        name: email
        description: optional email of member
      - in: query
        name: external_id
        description: optional external ID of member
      - in: query
        name: member_id
        description: optional ID of member
      responses:
        200:
          description: OK
      tags:
      - Member
      - Info
  /members/set_permissions:
    post:
      summary: Set Member Permissions
      description: Set member permissions.
      operationId: postMembersSetPermissions
      x-api-path-slug: membersset-permissions-post
      parameters:
      - in: query
        name: external_id
        description: optional external ID
      - in: query
        name: member_id
        description: optional member ID
      - in: query
        name: new_is_admin
        description: optional change the admin status of the member
      responses:
        200:
          description: OK
      tags:
      - Set
      - Member
      - Permissions