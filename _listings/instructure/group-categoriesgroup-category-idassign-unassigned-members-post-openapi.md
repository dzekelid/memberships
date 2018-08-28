---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Assign unassigned members
  description: Assign unassigned members.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/memberships:
    get:
      summary: List group memberships
      description: List group memberships.
      operationId: list-group-memberships
      x-api-path-slug: groupsgroup-idmemberships-get
      parameters:
      - in: query
        name: filter_states[]
        description: Only list memberships with the given workflow_states
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
    post:
      summary: Create a membership
      description: Create a membership.
      operationId: create-a-membership
      x-api-path-slug: groupsgroup-idmemberships-post
      parameters:
      - in: query
        name: user_id
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
  /groups/{group_id}/memberships/membership_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
  /group_categories/{group_category_id}/assign_unassigned_members:
    post:
      summary: Assign unassigned members
      description: Assign unassigned members.
      operationId: assign-unassigned-members
      x-api-path-slug: group-categoriesgroup-category-idassign-unassigned-members-post
      parameters:
      - in: query
        name: sync
        description: The assigning is done asynchronously by default
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Assign
      - Unassigned
      - Members
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