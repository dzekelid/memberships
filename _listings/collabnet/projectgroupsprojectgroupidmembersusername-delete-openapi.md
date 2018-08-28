---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Removes project group member
  version: 1.0.0
  description: Removes project group member.
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
  /groups/{groupid}/members:
    get:
      summary: Gets usergroup members
      description: Gets usergroup members.
      operationId: getUserGroupMembers
      x-api-path-slug: groupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
      responses:
        200:
          description: OK
      tags:
      - Usergroup
      - Members
  /users/{userid}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by user id
      description: Adds a user to specified project's member list by user id.
      operationId: addUserById
      x-api-path-slug: usersuseridprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
      - By
      - User
  /users/myself/projects/{projectid}:
    put:
      summary: Adds current user to specified project's member list
      description: Adds current user to specified project's member list.
      operationId: addMyself
      x-api-path-slug: usersmyselfprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
  /users/by-username/{username}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by username
      description: Adds a user to specified project's member list by username.
      operationId: addUserByUsername
      x-api-path-slug: usersbyusernameusernameprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
      - By
      - Username
  /projects/{projectid}/{username}:
    delete:
      summary: Removes project member
      description: Removes project member.
      operationId: removeProjectMember
      x-api-path-slug: projectsprojectidusername-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - Member
    put:
      summary: Adds project member
      description: Adds project member.
      operationId: addProjectMember
      x-api-path-slug: projectsprojectidusername-put
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Project
      - Member
  /projectgroups/{projectgroupid}/members/{username}:
    delete:
      summary: Removes project group member
      description: Removes project group member.
      operationId: removeProjectGroupMember
      x-api-path-slug: projectgroupsprojectgroupidmembersusername-delete
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - Group
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