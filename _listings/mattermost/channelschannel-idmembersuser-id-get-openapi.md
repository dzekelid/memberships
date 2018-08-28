---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get channel member
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{team_id}/members:
    get:
      summary: Get team members
      description: |-
        Get a page team members list based on query string parameters - team id, page and per page.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-page-team-members-list-based-on-query-string-parameters--team-id-page-and-per-page-permissions
      x-api-path-slug: teamsteam-idmembers-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of users per page
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Members
  /teams/{team_id}/members/ids:
    post:
      summary: Get team members by ids
      description: |-
        Get a list of team members based on a provided array of user ids.
        ##### Permissions
        Must have `view_team` permission for the team.
      operationId: get-a-list-of-team-members-based-on-a-provided-array-of-user-ids-permissionsmust-have-view-team-perm
      x-api-path-slug: teamsteam-idmembersids-post
      parameters:
      - in: body
        name: body
        description: List of user ids
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Members
      - By
      - Ids
  /channels/{channel_id}/members:
    get:
      summary: Get channel members
      description: |-
        Get a page of members for a channel.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: get-a-page-of-members-for-a-channel-permissionsread-channel-permission-for-the-channel
      x-api-path-slug: channelschannel-idmembers-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of members per page
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Members
  /channels/{channel_id}/members/ids:
    post:
      summary: Get channel members by ids
      description: |-
        Get a list of channel members based on the provided user ids.
        ##### Permissions
        Must have the `read_channel` permission.
      operationId: get-a-list-of-channel-members-based-on-the-provided-user-ids-permissionsmust-have-the-read-channel-p
      x-api-path-slug: channelschannel-idmembersids-post
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: body
        name: user_ids
        description: List of user ids
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Channel
      - Members
      - By
      - Ids
  /teams/{team_id}/members/{user_id}:
    get:
      summary: Get a team member
      description: |-
        Get a team member on the system.
        ##### Permissions
        Must be authenticated and have the `view_team` permission.
      operationId: get-a-team-member-on-the-system-permissionsmust-be-authenticated-and-have-the-view-team-permission
      x-api-path-slug: teamsteam-idmembersuser-id-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Member
  /teams/{team_id}/members/{user_id}/roles:
    put:
      summary: Update a team member roles
      description: |-
        Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
        ##### Permissions
        Must be authenticated and have the `manage_team_roles` permission.
      operationId: update-a-team-member-roles-valid-team-roles-are-team-user-team-admin-or-both-of-them-overwrites-any-
      x-api-path-slug: teamsteam-idmembersuser-idroles-put
      parameters:
      - in: body
        name: body
        description: Space-delimited team roles to assign to the user
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Team
      - Member
      - Roles
  /channels/{channel_id}/members/{user_id}:
    get:
      summary: Get channel member
      description: |-
        Get a channel member.
        ##### Permissions
        `read_channel` permission for the channel.
      operationId: get-a-channel-member-permissionsread-channel-permission-for-the-channel
      x-api-path-slug: channelschannel-idmembersuser-id-get
      parameters:
      - in: path
        name: channel_id
        description: Channel GUID
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - Channel
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