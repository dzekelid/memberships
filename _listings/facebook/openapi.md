swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{friendlist}/members:
    get:
      summary: Get Friendlist Members
      description: All of the users who are members of this list.
      operationId: getFriendlistMembers
      x-api-path-slug: friendlistmembers-get
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
  /{friendlist}/members/{user}:
    post:
      summary: Post Friendlist Members User
      description: Adds a user to the friend list
      operationId: postFriendlistMembersUser
      x-api-path-slug: friendlistmembersuser-post
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      - in: path
        name: user
        description: Represents the ID of the User to add to or remove from the friend
          list
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
      - User
    delete:
      summary: Delete Friendlist Members User
      description: Removes a user from the friend list
      operationId: deleteFriendlistMembersUser
      x-api-path-slug: friendlistmembersuser-delete
      parameters:
      - in: path
        name: friendlist
        description: Represents the ID of the FriendList object
      - in: path
        name: user
        description: Represents the ID of the User to add to or remove from the friend
          list
      responses:
        200:
          description: OK
      tags:
      - Friendlist
      - Members
      - User
  /{group}/members:
    get:
      summary: Get Group Members
      description: All of the users who are members of this group
      operationId: getGroupMembers
      x-api-path-slug: groupmembers-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members