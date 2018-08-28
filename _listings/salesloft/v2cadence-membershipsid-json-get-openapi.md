---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch a cadence membership
  description: Fetches a cadence membership, by ID only.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/cadence_memberships.json:
    get:
      summary: List cadence memberships
      description: |-
        Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to
        the respective parameters. A cadence membership is the association between a person and their current and
        historical time on a cadence. Cadence membership records are mutable and change over time. If a person is
        added to a cadence and re-added to the same cadence in the future, there is a single membership record.
      operationId: v2.cadence_memberships.json.get
      x-api-path-slug: v2cadence-memberships-json-get
      parameters:
      - in: query
        name: cadence_id
        description: ID of the cadence to find cadence memberships for
      - in: query
        name: ids
        description: IDs of cadence memberships to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: person_id
        description: ID of the person to find cadence memberships for
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Cadence
      - Memberships
    post:
      summary: Create a cadence membership
      description: |-
        Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will
        default to the authenticated user, but can be set to any visible user on the authenticated team.

        A person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by
        the teammate.
      operationId: v2.cadence_memberships.json.post
      x-api-path-slug: v2cadence-memberships-json-post
      parameters:
      - in: query
        name: cadence_id
        description: ID of the cadence to create a cadence membership for
      - in: query
        name: person_id
        description: ID of the person to create a cadence membership for
      - in: query
        name: user_id
        description: ID of the user to create a cadence membership for
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Cadence
      - Membership
  /v2/cadence_memberships/{id}.json:
    delete:
      summary: Delete a cadence membership
      description: ""
      operationId: v2.cadence_memberships.id.json.delete
      x-api-path-slug: v2cadence-membershipsid-json-delete
      parameters:
      - in: path
        name: id
        description: CadenceMembership ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Cadence
      - Membership
    get:
      summary: Fetch a cadence membership
      description: Fetches a cadence membership, by ID only.
      operationId: v2.cadence_memberships.id.json.get
      x-api-path-slug: v2cadence-membershipsid-json-get
      parameters:
      - in: path
        name: id
        description: CadenceMembership ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Cadence
      - Membership
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