---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Delete Projects Members User
  version: 1.0.0
  description: Removes a user from a group or project.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/groups/{id}/members:
    get:
      summary: Get Groups Members
      description: Gets a list of group or project members viewable by the authenticated
        user.
      operationId: getV3GroupsIdMembers
      x-api-path-slug: v3groupsidmembers-get
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: query
        description: A query string to search for members
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
    post:
      summary: Post Groups Members
      description: Adds a member to a group or project.
      operationId: postV3GroupsIdMembers
      x-api-path-slug: v3groupsidmembers-post
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The group ID
      - in: formData
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
  /v3/groups/{id}/members/{user_id}:
    get:
      summary: Get Groups Members User
      description: Gets a member of a group or project.
      operationId: getV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-get
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
    put:
      summary: Put Groups Members User
      description: Updates a member of a group or project.
      operationId: putV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-put
      parameters:
      - in: formData
        name: access_level
        description: A valid access level
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
    delete:
      summary: Delete Groups Members User
      description: Removes a user from a group or project.
      operationId: deleteV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-delete
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
  /v3/projects/{id}/members:
    get:
      summary: Get Projects Members
      description: Gets a list of group or project members viewable by the authenticated
        user.
      operationId: getV3ProjectsIdMembers
      x-api-path-slug: v3projectsidmembers-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: query
        description: A query string to search for members
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
    post:
      summary: Post Projects Members
      description: Adds a member to a group or project.
      operationId: postV3ProjectsIdMembers
      x-api-path-slug: v3projectsidmembers-post
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
  /v3/projects/{id}/members/{user_id}:
    get:
      summary: Get Projects Members User
      description: Gets a member of a group or project.
      operationId: getV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
      - User
    put:
      summary: Put Projects Members User
      description: Updates a member of a group or project.
      operationId: putV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-put
      parameters:
      - in: formData
        name: access_level
        description: A valid access level
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
      - User
    delete:
      summary: Delete Projects Members User
      description: Removes a user from a group or project.
      operationId: deleteV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-delete
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
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