---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Get team members
  x-api-slug: teamsteam-idmembers-get
  description: |-
    Get a page team members list based on query string parameters - team id, page and per page.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembers-get-openapi.md
- name: Mattermost API Reference - Get team members by ids
  x-api-slug: teamsteam-idmembersids-post
  description: |-
    Get a list of team members based on a provided array of user ids.
    ##### Permissions
    Must have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get a team member
  x-api-slug: teamsteam-idmembersuser-id-get
  description: |-
    Get a team member on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Update a team member roles
  x-api-slug: teamsteam-idmembersuser-idroles-put
  description: |-
    Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
    ##### Permissions
    Must be authenticated and have the `manage_team_roles` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Get channel members by ids
  x-api-slug: channelschannel-idmembersids-post
  description: |-
    Get a list of channel members based on the provided user ids.
    ##### Permissions
    Must have the `read_channel` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get channel members
  x-api-slug: channelschannel-idmembers-get
  description: |-
    Get a page of members for a channel.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembers-get-openapi.md
- name: Mattermost API Reference - Get team members by ids
  x-api-slug: teamsteam-idmembersids-post
  description: |-
    Get a list of team members based on a provided array of user ids.
    ##### Permissions
    Must have `view_team` permission for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersids-post-openapi.md
- name: Mattermost API Reference - Get team members
  x-api-slug: teamsteam-idmembers-get
  description: |-
    Get a page team members list based on query string parameters - team id, page and per page.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembers-get-openapi.md
- name: Mattermost API Reference - Get channel member
  x-api-slug: channelschannel-idmembersuser-id-get
  description: |-
    Get a channel member.
    ##### Permissions
    `read_channel` permission for the channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/channelschannel-idmembersuser-id-get-openapi.md
- name: Mattermost API Reference - Update a team member roles
  x-api-slug: teamsteam-idmembersuser-idroles-put
  description: |-
    Update a team member roles. Valid team roles are "team_user", "team_admin" or both of them. Overwrites any previously assigned team roles.
    ##### Permissions
    Must be authenticated and have the `manage_team_roles` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersuser-idroles-put-openapi.md
- name: Mattermost API Reference - Get a team member
  x-api-slug: teamsteam-idmembersuser-id-get
  description: |-
    Get a team member on the system.
    ##### Permissions
    Must be authenticated and have the `view_team` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/mattermost/teamsteam-idmembersuser-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---