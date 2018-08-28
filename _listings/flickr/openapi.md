swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
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