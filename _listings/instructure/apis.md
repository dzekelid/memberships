---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Memberships
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Groups API List group memberships
  x-api-slug: instructure-canvas-groups-api
  description: List group memberships.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmemberships-get-openapi.md
- name: Instructure Canvas Groups API Create a membership
  x-api-slug: instructure-canvas-groups-api
  description: Create a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmemberships-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmemberships-post-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-openapi.md
- name: Instructure Canvas Groups API
  x-api-slug: instructure-canvas-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Memberships
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---