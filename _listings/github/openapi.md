---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers--over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories--with-the-collaborative-features-of-github-com-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code-
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{teamId}/memberships/{username}:
    delete:
      summary: Delete Teams Team Memberships Username
      description: |-
        Remove team membership.
        In order to remove a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with. NOTE: This does not delete the user, it just removes their membership from the team.
      operationId: remove-team-membershipin-order-to-remove-a-membership-between-a-user-and-a-team-the-authenticated-us
      x-api-path-slug: teamsteamidmembershipsusername-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      - in: path
        name: username
        description: Name of a member
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Memberships
      - Username
    get:
      summary: Get Teams Team Memberships Username
      description: |-
        Get team membership.
        In order to get a user's membership with a team, the authenticated user must be a member of the team or an owner of the team's organization.
      operationId: get-team-membershipin-order-to-get-a-users-membership-with-a-team-the-authenticated-user-must-be-a-m
      x-api-path-slug: teamsteamidmembershipsusername-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      - in: path
        name: username
        description: Name of a member
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Memberships
      - Username
    put:
      summary: Put Teams Team Memberships Username
      description: |-
        Add team membership.
        In order to add a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with.

        If the user is already a part of the team's organization (meaning they're on at least one other team in the organization), this endpoint will add the user to the team.

        If the user is completely unaffiliated with the team's organization (meaning they're on none of the organization's teams), this endpoint will send an invitation to the user via email. This newly-created membership will be in the 'pending' state until the user accepts the invitation, at which point the membership will transition to the 'active' state and the user will be added as a member of the team.
      operationId: add-team-membershipin-order-to-add-a-membership-between-a-user-and-a-team-the-authenticated-user-mus
      x-api-path-slug: teamsteamidmembershipsusername-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: teamId
        description: Id of team
      - in: path
        name: username
        description: Name of a member
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Team
      - Memberships
      - Username
---