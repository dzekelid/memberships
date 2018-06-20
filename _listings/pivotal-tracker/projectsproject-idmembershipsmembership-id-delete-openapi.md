---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 0
info:
  title: Pivotal Tracker Delete Projects Project Memberships Membership
  description: Delete projects project memberships membership.
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{PROJECT_ID}/memberships:
    get:
      summary: Get Projects Project Memberships
      description: Retrieves all memberships for a project.
      operationId: getProjectsProjectMemberships
      x-api-path-slug: projectsproject-idmemberships-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
    post:
      summary: Post Projects Project Memberships
      description: Adds a new membership to a project.
      operationId: postProjectsProjectMemberships
      x-api-path-slug: projectsproject-idmemberships-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
  /projects/{PROJECT_ID}/memberships/{MEMBERSHIP_ID}:
    get:
      summary: Get Projects Project Memberships Membership
      description: Retrieves information about a single membership.
      operationId: getProjectsProjectMembershipsMembership
      x-api-path-slug: projectsproject-idmembershipsmembership-id-get
      parameters:
      - in: path
        name: MEMBERSHIP_ID
        description: The ID of the membership
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
      - MEMBERSHIP
      - ID
    delete:
      summary: Delete Projects Project Memberships Membership
      description: Delete projects project memberships membership.
      operationId: deleteProjectsProjectMembershipsMembership
      x-api-path-slug: projectsproject-idmembershipsmembership-id-delete
      parameters:
      - in: path
        name: MEMBERSHIP_ID
        description: The ID of the membership
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Memberships
      - MEMBERSHIP
      - ID
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