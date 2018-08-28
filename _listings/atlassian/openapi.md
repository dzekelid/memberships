swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /group/{groupName}/member:
    get:
      summary: Get group members
      description: |-
        Returns the users that are members of a group.

        **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
        Permission to access the Confluence site ('Can use' global permission).
      operationId: com.atlassian.confluence.plugins.restapi.resources.GroupResource.getGroupMembers_get
      x-api-path-slug: groupgroupnamemember-get
      parameters:
      - in: path
        name: groupName
        description: The name of the group to be queried for its members
      - in: query
        name: limit
        description: The maximum number of users to return per page
      - in: query
        name: start
        description: The starting index of the returned users
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members
  /api/2/role:
    get:
      summary: Get all project roles
      description: |-
        Gets a list of all project roles, complete with project role details and default actors.

        ### About project roles

        [Project roles](https://confluence.atlassian.com/x/3odKLg) are a flexible way to to associate users and groups with projects. In Jira Cloud, the list of project roles is shared globally with all projects, but each project can have a different set of actors associated with it (unlike groups, which have the same membership throughout all Jira applications).

        Project roles can be used in [permission schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-permissionscheme-get), [email notification schemes](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-notificationscheme-get), [issue security levels](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-issuesecurityschemes-get), [comment visibility](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-comment-list-post), and workflow conditions.

        #### Members and actors

        In the Jira REST API, a member of a project role is called an _actor_. An _actor_ is a group or user associated with a project role.

        Actors may be set as [default members](https://confluence.atlassian.com/x/3odKLg#Managingprojectroles-Specifying'defaultmembers'foraprojectrole) of the project role or set at the project level:

        *   Default actors: Users and groups that are assigned to the project role for all newly created projects. The default actors can be removed at the project level later if desired.
        *   Actors: Users and groups that are associated with a project role for a particular project, which may differ from the default actors. This allows you to assign a particular user to different roles in different projects.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ [global permission](https://confluence.atlassian.com/x/x4dKLg).
      operationId: com.atlassian.jira.rest.v2.issue.project.RoleResource.getAllProjectRoles_get
      x-api-path-slug: api2role-get
      responses:
        200:
          description: OK
      tags:
      - Project
      - Roles