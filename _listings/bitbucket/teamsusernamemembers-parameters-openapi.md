---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Teams Username Members
  description: Parameters teams username members
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{username}/members:
    get:
      summary: Get Teams Username Members
      description: |-
        All members of a team.

        Returns all members of the specified team. Any member of any of the
        team's groups is considered a member of the team. This includes users
        in groups that may not actually have access to any of the team's
        repositories.

        Note that members using the "private profile" feature are not included.
      operationId: getTeamsUsernameMembers
      x-api-path-slug: teamsusernamemembers-get
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Members
    parameters:
      summary: Parameters Teams Username Members
      description: Parameters teams username members
      operationId: parametersTeamsUsernameMembers
      x-api-path-slug: teamsusernamemembers-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
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