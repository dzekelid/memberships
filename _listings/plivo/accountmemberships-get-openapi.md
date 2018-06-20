---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Get Account Memberships
  description: ID of a user should be specified as a query parameter. JSON with membership
    details is returned. For this API call system/admin or system/manager role is
    required
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/memberships:
    get:
      summary: Get Account Memberships
      description: ID of a user should be specified as a query parameter. JSON with
        membership details is returned. For this API call system/admin or system/manager
        role is required
      operationId: getMembershipsOfSpecificUser
      x-api-path-slug: accountmemberships-get
      parameters:
      - in: query
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Memberships
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