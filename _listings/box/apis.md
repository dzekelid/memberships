---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "445"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box - Create Membership
  x-api-slug: group-memberships-post
  description: Used to add a member to a Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-memberships-post-openapi.md
- name: Box - Get Membership
  x-api-slug: group-membershipsgroup-membership-id-get
  description: Fetches a specific group membership entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-openapi.md
- name: Box - Update Membership
  x-api-slug: group-membershipsgroup-membership-id-put
  description: Used to update a group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-put-openapi.md
- name: Box - Delete Membership
  x-api-slug: group-membershipsgroup-membership-id-delete
  description: Deletes a specific group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-openapi.md
- name: Box - Get Memberships for Group
  x-api-slug: groupsgroup-idmemberships-get
  description: Retrieves all of the members for a given group if the requesting user
    has access (see Group Object member_viewability_level).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/groupsgroup-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/groupsgroup-idmemberships-get-openapi.md
- name: Box - Get Memberships for User
  x-api-slug: usersuser-idmemberships-get
  description: Retrieves all of the group memberships for a given user. Note this
    is only available to group admins. To retrieve group memberships for the user
    making the API request, use the users/me/memberships endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/usersuser-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/usersuser-idmemberships-get-openapi.md
- name: Box - Get Membership
  x-api-slug: group-membershipsgroup-membership-id-get
  description: Fetches a specific group membership entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-openapi.md
- name: Box - Update Membership
  x-api-slug: group-membershipsgroup-membership-id-put
  description: Used to update a group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-put-openapi.md
- name: Box - Delete Membership
  x-api-slug: group-membershipsgroup-membership-id-delete
  description: Deletes a specific group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-openapi.md
- name: Box - Delete Membership
  x-api-slug: group-membershipsgroup-membership-id-delete
  description: Deletes a specific group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-delete-openapi.md
- name: Box - Update Membership
  x-api-slug: group-membershipsgroup-membership-id-put
  description: Used to update a group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-put-openapi.md
- name: Box - Get Membership
  x-api-slug: group-membershipsgroup-membership-id-get
  description: Fetches a specific group membership entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/box/group-membershipsgroup-membership-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://botify.api.gallery.streamdata.io
- type: x-api-stack
  url: http://box.stack.network
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/box
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---