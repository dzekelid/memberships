---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 0
info:
  title: Mailgun API List Member
  description: Retrieves a mailing list member.
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  lists/{address}/members/:
    get:
      summary: List Members
      description: Fetches the list of mailing list members.
      operationId: getListsAddressMembers
      x-api-path-slug: listsaddressmembers-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: skip
        description: Records to skip (0 by default)
      - in: query
        name: subscribed
        description: yes to list subscribed, no for unsubscribed, list all if not
          set
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  lists/{address}/members/{member_address}:
    get:
      summary: List Member
      description: Retrieves a mailing list member.
      operationId: getListsAddressMembersMemberAddress
      x-api-path-slug: listsaddressmembersmember-address-get
      parameters:
      - in: query
        name: address
        description: Email address of commenter
      - in: query
        name: member_address
        description: Email address on the list
      responses:
        200:
          description: OK
      tags:
      - List
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