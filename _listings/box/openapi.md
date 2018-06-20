---
swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  description: the-box-content-api-gives-you-access-to-secure-content-management-and-content-experience-features-for-use-in-your-own-app--it-strives-to-be-restful-and-is-organized-around-the-main-resources-youre-familiar-with-from-the-box-web-interface-
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
    delete:
      summary: Delete Membership
      description: Deletes a specific group membership.
      operationId: deleteGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-delete
      parameters:
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
  /groups/{GROUP_ID}/memberships:
    get:
      summary: Get Memberships for Group
      description: Retrieves all of the members for a given group if the requesting
        user has access (see Group Object member_viewability_level).
      operationId: getGroupMemberships
      x-api-path-slug: groupsgroup-idmemberships-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_ID
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
      - ""
      - Memberships
  /users/{USER_ID}/memberships:
    get:
      summary: Get Memberships for User
      description: Retrieves all of the group memberships for a given user. Note this
        is only available to group admins. To retrieve group memberships for the user
        making the API request, use the users/me/memberships endpoint.
      operationId: getUserGroupMembership
      x-api-path-slug: usersuser-idmemberships-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: limit
        description: Default is 100
      - in: query
        name: offset
        description: The item at which to begin the response
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Users
      - User
      - ""
      - Memberships
---