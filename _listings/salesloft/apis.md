---
name: SalesLoft
x-slug: salesloft
description: SalesLoft, the leading sales engagement platform, transforms the way
  sellers engage with their customers by delivering a better selling experience. Our
  sales engagement platform helps teams set and execute on a cadence of phone, email,
  and social communications to convert more target accounts into customer accounts.
  The platform equips sales leaders with new capabilities to test, learn and adapt
  to ensure their sales reps execute on the most effective selling process for their
  account-based approach. SalesLoft delivers access to an extensive ecosystem of 3rd
  party integrations allowing teams to perform all their sales engagement from a single
  platform.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/apis.md
specificationVersion: "0.14"
apis:
- name: SalesLoft - List cadence memberships
  x-api-slug: v2cadence-memberships-json-get
  description: |-
    Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to
    the respective parameters. A cadence membership is the association between a person and their current and
    historical time on a cadence. Cadence membership records are mutable and change over time. If a person is
    added to a cadence and re-added to the same cadence in the future, there is a single membership record.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-get-openapi.md
- name: SalesLoft - Create a cadence membership
  x-api-slug: v2cadence-memberships-json-post
  description: |-
    Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will
    default to the authenticated user, but can be set to any visible user on the authenticated team.

    A person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by
    the teammate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-post-openapi.md
- name: SalesLoft - Delete a cadence membership
  x-api-slug: v2cadence-membershipsid-json-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-delete-openapi.md
- name: SalesLoft - Fetch a cadence membership
  x-api-slug: v2cadence-membershipsid-json-get
  description: Fetches a cadence membership, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-get-openapi.md
- name: SalesLoft - Fetch a cadence membership
  x-api-slug: v2cadence-membershipsid-json-get
  description: Fetches a cadence membership, by ID only.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-get-openapi.md
- name: SalesLoft - Delete a cadence membership
  x-api-slug: v2cadence-membershipsid-json-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-membershipsid-json-delete-openapi.md
- name: SalesLoft - Create a cadence membership
  x-api-slug: v2cadence-memberships-json-post
  description: |-
    Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will
    default to the authenticated user, but can be set to any visible user on the authenticated team.

    A person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by
    the teammate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/salesloft.png
  humanURL: http://salesloft.com
  baseURL: https://api.salesloft.com//
  tags: Sales, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/salesloft/v2cadence-memberships-json-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://salesforce.api.gallery.streamdata.io
- type: x-api-stack
  url: http://salesloft.stack.network
- type: x-blog
  url: https://salesloft.com/resources/blog/
- type: x-blog-rss
  url: https://salesloft.com/feed/
- type: x-developer
  url: https://developers.salesloft.com/api.html
- type: x-documentation
  url: https://developers.salesloft.com/api.html#!/Topic/Introduction
- type: x-github
  url: https://github.com/SalesLoft
- type: x-pricing
  url: https://salesloft.com/plans/
- type: x-support
  url: https://salesloft.com/support/
- type: x-twitter
  url: https://twitter.com/SalesLoft
- type: x-website
  url: http://salesloft.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---