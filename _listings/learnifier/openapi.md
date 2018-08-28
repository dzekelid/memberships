swagger: "2.0"
x-collection-name: Learnifier
x-complete: 1
info:
  title: Learnifier
  version: 1.1.0
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orgunits/{orgid}/projects/{projectid}/teammembers:
    get:
      summary: Project team members
      description: Returns the project team members. A team member is a ....
      operationId: orgunits.orgid.projects.projectid.teammembers.get
      x-api-path-slug: orgunitsorgidprojectsprojectidteammembers-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Team
      - Members
  /orgunits/{orgid}/usergroups/{groupid}/members:
    get:
      summary: List of all users in group.
      description: Returns a list of all members in User Groups that are based on
        the Global Group with this groupid.
      operationId: orgunits.orgid.usergroups.groupid.members.get
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members
    post:
      summary: Add user group member.
      description: Adds a user to user group.
      operationId: orgunits.orgid.usergroups.groupid.members.post
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members
  /orgunits/{orgid}/usergroups/{groupid}/members/{uuid}:
    delete:
      summary: Remove user group member.
      description: Removes a user from a user group.
      operationId: orgunits.orgid.usergroups.groupid.members.uuid.delete
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembersuuid-delete
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      - in: path
        name: uuid
        description: UUID of user to remove from group
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members