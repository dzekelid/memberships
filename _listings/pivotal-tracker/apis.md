---
name: Pivotal Tracker
x-slug: pivotal-tracker
description: Writing software isn&rsquo;t half as hard as all the talking, emails,
  and meetings needed to reconcile shifting requirements and slipping deadlines. We
  get it, we&rsquo;ve been there. In fact, we&rsquo;re still there. Were Pivotal Labs,
  a web and mobile development consultancy. In 2006 we built Tracker for our developers
  and clients to facilitate constructive communication, reflect the status of a project
  and help forecast its future. Today Tracker is a staple of the developers toolkit.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Memberships
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/apis.md
specificationVersion: "0.14"
apis:
- name: Pivotal Tracker Get Projects Project Memberships
  x-api-slug: pivotal-tracker
  description: Retrieves all memberships for a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
  humanURL: http://pivotaltracker.com
  baseURL: https://www.pivotaltracker.com//services/v3///projects/{PROJECT_ID}/memberships
  tags: Projects,PROJECT,ID,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmemberships-get-openapi.md
- name: Pivotal Tracker Post Projects Project Memberships
  x-api-slug: pivotal-tracker
  description: Adds a new membership to a project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
  humanURL: http://pivotaltracker.com
  baseURL: https://www.pivotaltracker.com//services/v3///projects/{PROJECT_ID}/memberships
  tags: Projects,PROJECT,ID,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmemberships-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmemberships-post-openapi.md
- name: Pivotal Tracker Get Projects Project Memberships Membership
  x-api-slug: pivotal-tracker
  description: Retrieves information about a single membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
  humanURL: http://pivotaltracker.com
  baseURL: https://www.pivotaltracker.com//services/v3///projects/{PROJECT_ID}/memberships/{MEMBERSHIP_ID}
  tags: Projects,PROJECT,ID,Memberships,MEMBERSHIP,ID
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmembershipsmembership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmembershipsmembership-id-get-openapi.md
- name: Pivotal Tracker Delete Projects Project Memberships Membership
  x-api-slug: pivotal-tracker
  description: Delete projects project memberships membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
  humanURL: http://pivotaltracker.com
  baseURL: https://www.pivotaltracker.com//services/v3///projects/{PROJECT_ID}/memberships/{MEMBERSHIP_ID}
  tags: Projects,PROJECT,ID,Memberships,MEMBERSHIP,ID
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmembershipsmembership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/projectsproject-idmembershipsmembership-id-delete-openapi.md
- name: Pivotal Tracker
  x-api-slug: pivotal-tracker
  description: Whether welding together two apps or forging a unique one, tap into
    100% of the Tracker feature set with the very same API the Tracker team uses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/pivotal-tracker.png
  humanURL: http://pivotaltracker.com
  baseURL: https://www.pivotaltracker.com//services/v3/
  tags: Memberships
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/pivotal-tracker/openapi.md
x-common:
- type: x-blog
  url: http://www.pivotaltracker.com/community/tracker-blog
- type: x-blog
  url: http://www.pivotaltracker.com/feed
- type: x-email
  url: TRACKER@PIVOTAL.IO
- type: x-faq
  url: https://www.pivotaltracker.com/faq
- type: x-github
  url: https://github.com/pivotal
- type: x-pricing
  url: http://www.pivotaltracker.com/why-tracker/pricing
- type: x-selfservice-registration
  url: https://www.pivotaltracker.com/signup/new
- type: x-status
  url: http://status.pivotaltracker.com/
- type: x-terms-of-service
  url: https://www.pivotaltracker.com/policy/eula
- type: x-twitter
  url: https://twitter.com/pivotaltracker
- type: x-website
  url: http://pivotaltracker.com
- type: x-website
  url: http://www.pivotaltracker.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---