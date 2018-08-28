---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Delete Memberships
  description: Delete a membership. It requires the **administrator** or **project
    creator** global role or the **project owner** role on the project.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /memberships:
    delete:
      summary: Delete Memberships
      description: Delete a membership. It requires the **administrator** or **project
        creator** global role or the **project owner** role on the project.
      operationId: DeleteMember
      x-api-path-slug: memberships-delete
      parameters:
      - in: body
        name: membership
        description: Delete membership
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
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