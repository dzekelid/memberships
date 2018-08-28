---
name: Cisco WebEx
x-slug: cisco-webex
description: Cisco Webex is the leading enterprise solution for video conferencing
  & web conferencing today. This secure software-based platform for video & audio
  conferencing, group messaging & webinars helps organizations be more productive.Participants
  can join ...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
x-kinRank: "7"
x-alexaRank: "632"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/apis.md
specificationVersion: "0.14"
apis:
- name: Webex Teams API - List memberships (for all rooms)
  x-api-slug: memberships-get
  description: |-
    Lists all room memberships. By default, lists memberships for rooms to which the authenticated user belongs.

    Use query parameters to filter the response.

    Use roomId to list memberships for a room, by ID.

    Use either personId or personEmail to filter the results.

    https://developer.webex.com/endpoint-memberships-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-get-openapi.md
- name: Webex Teams API - List team memberships
  x-api-slug: teammemberships-get
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-get-openapi.md
- name: Webex Teams API - Get membership details
  x-api-slug: memberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-get-openapi.md
- name: Webex Teams API - Update a membership
  x-api-slug: memberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-put-openapi.md
- name: Webex Teams API - Delete membership
  x-api-slug: memberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-delete-openapi.md
- name: Webex Teams API - Create a membership
  x-api-slug: memberships-post
  description: |-
    Add someone to a room by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-memberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-post-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Create a membership
  x-api-slug: memberships-post
  description: |-
    Add someone to a room by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-memberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-post-openapi.md
- name: Webex Teams API - Create a membership
  x-api-slug: memberships-post
  description: |-
    Add someone to a room by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-memberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-post-openapi.md
- name: Webex Teams API - Delete membership
  x-api-slug: memberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-delete-openapi.md
- name: Webex Teams API - Delete membership
  x-api-slug: memberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-delete-openapi.md
- name: Webex Teams API - Update a membership
  x-api-slug: memberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-put-openapi.md
- name: Webex Teams API - Update a membership
  x-api-slug: memberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-put-openapi.md
- name: Webex Teams API - Get membership details
  x-api-slug: memberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-get-openapi.md
- name: Webex Teams API - Get membership details
  x-api-slug: memberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/cisco-webex/memberships-membership-get-openapi.md
x-common:
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/1f5e101d8290a5303c90
- type: x-api-gallery
  url: http://cisco.unity.connection.messaging.interface.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cisco.webex.stack.network
- type: x-blog
  url: http://blogs.webex.com/
- type: x-blog-rss
  url: http://blogs.webex.com/webex_interactions/index.rdf
- type: x-crunchbase
  url: https://crunchbase.com/organization/webex-communications
- type: x-crunchbase
  url: http://www.crunchbase.com/company/webex
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/0aa22af74405f82086d4
- type: x-twitter
  url: https://twitter.com/webex
- type: x-developer
  url: https://developer.webex.com/
- type: x-website
  url: https://webex.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---