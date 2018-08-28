---
name: Hewlett Packard Enterprise (HPE)
x-slug: hewlett-packard-enterprise-hpe
description: We help customers use technology to slash the time it takes to turn ideas
  into value. In turn, they transform industries, markets and lives. Some of our customers
  run traditional IT environments. Most are transitioning to a secure, cloud-enabled,
  mobile-friendly infrastructure. Many rely on a combination of both. Wherever they
  are in that journey, we provide the technology and solutions to help them succeed.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/apis.md
specificationVersion: "0.14"
apis:
- name: HPE OneSphere API - Delete Memberships
  x-api-slug: memberships-delete
  description: Delete a membership. It requires the **administrator** or **project
    creator** global role or the **project owner** role on the project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/memberships-delete-openapi.md
- name: HPE OneSphere API - Get Memberships
  x-api-slug: memberships-get
  description: |-
    Returns memberships. Supports filtering by projectUri, userUri, userGroupUri, roleUri (but only
    individual values, not multiple) in 'query'.

    If projectURI and userUri/userGroupUri are given a different
    backend path will be used that should be authorized to a project owner even if they wouldn't ordinarily
    be able to see other users' roles.

    It requires the **administrator** or **project creator** global role or the **project owner** role on the project.
    **project owner** requires **projectUri** to be supplied.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/memberships-get-openapi.md
- name: HPE OneSphere API - Post Memberships
  x-api-slug: memberships-post
  description: Creates a new membership. It requires the **administrator** or **project
    creator** global role or **project owner** role on the project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/memberships-post-openapi.md
- name: HPE OneSphere API - Get Membership Roles
  x-api-slug: membershiproles-get
  description: Returns membership (project-specific) roles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/membershiproles-get-openapi.md
- name: HPE OneSphere API - Get Membership Roles
  x-api-slug: membershiproles-get
  description: Returns membership (project-specific) roles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/membershiproles-get-openapi.md
- name: HPE OneSphere API - Get Membership Roles
  x-api-slug: membershiproles-get
  description: Returns membership (project-specific) roles.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/hewlett-packard-enterprise-hpe/membershiproles-get-openapi.md
x-common:
- type: x-developer
  url: https://developer.hpe.com/
- type: x-github
  url: https://github.com/hewlettpackard
- type: x-openapi
  url: https://raw.githubusercontent.com/HewlettPackard/hpe-onesphere-http/master/swagger.yml
- type: x-twitter
  url: https://twitter.com/HPE
- type: x-website
  url: http://HPE.com
- type: x-api-gallery
  url: http://heroku.api.gallery.streamdata.io
- type: x-api-stack
  url: http://hewlett.packard.enterprise.hpe.stack.network
- type: x-blog
  url: https://developer.hpe.com/blog
- type: x-curated-source
  url: http://community.hpe.com/t5/LoadRunner-and-Performance/LoadRunner-and-VuGen-12-53-load-testing-software-What-s-new-in/ba-p/6885101
- type: x-website
  url: https://www.hpe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---