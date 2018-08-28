---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Groups Members Get List
  description: Get a list of the members of a group. The call must be signed on behalf
    of a Flickr member, and the ability to see the group membership will be determined
    by the Flickr member's group privileges.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.groups.members.getList:
    get:
      summary: Groups Members Get List
      description: Get a list of the members of a group. The call must be signed on
        behalf of a Flickr member, and the ability to see the group membership will
        be determined by the Flickr member's group privileges.
      operationId: getRestMethodFlickr.groups.members.getlist
      x-api-path-slug: restmethodflickr-groups-members-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: group_id
        description: Return a list of members for this group
      - in: query
        name: membertypes
        description: Comma separated list of member types
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of groups to return per page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - GetList
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