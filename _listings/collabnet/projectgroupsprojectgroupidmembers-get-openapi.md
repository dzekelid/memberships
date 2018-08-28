---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets project group members
  version: 1.0.0
  description: Gets project group members.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /roles/{roleid}/members:
    get:
      summary: Gets role members
      description: Gets role members.
      operationId: getRoleMembers
      x-api-path-slug: rolesroleidmembers-get
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Role
      - Members
  /projects/{projectid}/roles/{roleid}/members:
    get:
      summary: Gets project role members
      description: Gets project role members.
      operationId: getProjectRoleMembers
      x-api-path-slug: projectsprojectidrolesroleidmembers-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
      - Members
  /projects/{projectid}/members:
    get:
      summary: Gets project members
      description: Gets project members.
      operationId: getProjectMembers
      x-api-path-slug: projectsprojectidmembers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
      - in: path
        name: projectid
        description: Project identifier
      - in: query
        name: searchvalue
        description: Filter value for project member name
      - in: query
        name: sortby
        description: Sorting column name
      responses:
        200:
          description: OK
      tags:
      - Project
      - Members
  /projectgroups/{projectgroupid}/members:
    get:
      summary: Gets project group members
      description: Gets project group members.
      operationId: getProjectGroupMembers
      x-api-path-slug: projectgroupsprojectgroupidmembers-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
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