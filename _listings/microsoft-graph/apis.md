---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph API - List Members
  x-api-slug: directoryrolesidmembers-get
  description: List members Retrieve a list of the users that are assigned to the
    directory role.  Only users can be assigned to a directory role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembers-get-openapi.md
- name: Microsoft Graph API - List Members
  x-api-slug: groupsidmembers-get
  description: List members Get a list of the group's direct members. A group can
    have users, contacts, and other groups as members. This operation is not transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembers-get-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: mecheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/mecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/mecheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: usersid--userprincipalnamecheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Group Check Member Groups
  x-api-slug: groupsidcheckmembergroups-post
  description: 'group: checkMemberGroups Check for membership in the specified list
    of groups. Returns from the list those groups of which the specified group has
    a direct or transitive membership.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: directoryobjectsidcheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: megetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: usersid--userprincipalnamegetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-openapi.md
- name: Microsoft Graph API - Group Get Member Groups
  x-api-slug: groupsidgetmembergroups-post
  description: 'group: getMemberGroups Return all the groups that the specified group
    is a member of. The check is transitive, unlike reading the memberOf navigation
    property, which returns only the groups that the group is a direct member of.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: directoryobjectsidgetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: megetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: usersid--userprincipalnamegetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: directoryobjectsidgetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Add Directory Role Member
  x-api-slug: directoryrolesidmembersref-post
  description: Add directory role member Use this API to create a new directory role
    member.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembersref-post-openapi.md
- name: Microsoft Graph API - Remove Member
  x-api-slug: groupsidmembersidref-delete
  description: Remove member Use this API to remove a member from an Office 365 group,
    a security group or a mail-enabled security group through the members navigation
    property. You can remove users or other groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersidref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersidref-delete-openapi.md
- name: Microsoft Graph API - Group Get Member Objects
  x-api-slug: groupsidgetmemberobjects-post
  description: 'group: getMemberObjects Return all of the groups that this group is
    a member of. The check is transitive. Note: Groups cannot be members of directory
    roles, so no directory roles will be returned.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - List Member Of
  x-api-slug: groupsidmemberof-get
  description: List memberOf Get groups that the group is a direct member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmemberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmemberof-get-openapi.md
- name: Microsoft Graph API - Add Member
  x-api-slug: groupsidmembersref-post
  description: 'Add member Use this API to add a member to an Office 365 group, a
    security group or a mail-enabled security group through the members navigation
    property. You can add users or other groups. Important: You can add only users
    to Office 365 groups.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersref-post-openapi.md
- name: Microsoft Graph API - List Member Of
  x-api-slug: usersid--userprincipalnamememberof-get
  description: List memberOf Get groups and directory roles that the user is a direct
    member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamememberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamememberof-get-openapi.md
- name: Microsoft Graph API - List Members
  x-api-slug: groupsidmembers-get
  description: List members Get a list of the group's direct members. A group can
    have users, contacts, and other groups as members. This operation is not transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembers-get-openapi.md
- name: Microsoft Graph API - List Members
  x-api-slug: directoryrolesidmembers-get
  description: List members Retrieve a list of the users that are assigned to the
    directory role.  Only users can be assigned to a directory role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembers-get-openapi.md
- name: Microsoft Graph API - List Member Of
  x-api-slug: usersid--userprincipalnamememberof-get
  description: List memberOf Get groups and directory roles that the user is a direct
    member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamememberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamememberof-get-openapi.md
- name: Microsoft Graph API - Add Member
  x-api-slug: groupsidmembersref-post
  description: 'Add member Use this API to add a member to an Office 365 group, a
    security group or a mail-enabled security group through the members navigation
    property. You can add users or other groups. Important: You can add only users
    to Office 365 groups.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersref-post-openapi.md
- name: Microsoft Graph API - List Member Of
  x-api-slug: groupsidmemberof-get
  description: List memberOf Get groups that the group is a direct member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmemberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmemberof-get-openapi.md
- name: Microsoft Graph API - Group Get Member Objects
  x-api-slug: groupsidgetmemberobjects-post
  description: 'group: getMemberObjects Return all of the groups that this group is
    a member of. The check is transitive. Note: Groups cannot be members of directory
    roles, so no directory roles will be returned.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Remove Member
  x-api-slug: groupsidmembersidref-delete
  description: Remove member Use this API to remove a member from an Office 365 group,
    a security group or a mail-enabled security group through the members navigation
    property. You can remove users or other groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersidref-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidmembersidref-delete-openapi.md
- name: Microsoft Graph API - Add Directory Role Member
  x-api-slug: directoryrolesidmembersref-post
  description: Add directory role member Use this API to create a new directory role
    member.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembersref-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryrolesidmembersref-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: directoryobjectsidgetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: usersid--userprincipalnamegetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Objects
  x-api-slug: megetmemberobjects-post
  description: Get member objects Returns all the groups and directory roles that
    a user, group, or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmemberobjects-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmemberobjects-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: directoryobjectsidgetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-openapi.md
- name: Microsoft Graph API - Group Get Member Groups
  x-api-slug: groupsidgetmembergroups-post
  description: 'group: getMemberGroups Return all the groups that the specified group
    is a member of. The check is transitive, unlike reading the memberOf navigation
    property, which returns only the groups that the group is a direct member of.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidgetmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: usersid--userprincipalnamegetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-openapi.md
- name: Microsoft Graph API - Get Member Groups
  x-api-slug: megetmembergroups-post
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/megetmembergroups-post-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: directoryobjectsidcheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Group Check Member Groups
  x-api-slug: groupsidcheckmembergroups-post
  description: 'group: checkMemberGroups Check for membership in the specified list
    of groups. Returns from the list those groups of which the specified group has
    a direct or transitive membership.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: usersid--userprincipalnamecheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-openapi.md
- name: Microsoft Graph API - Check Member Groups
  x-api-slug: mecheckmembergroups-post
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Microsoft, Files, Notes, Tasks, Stack Network, API Provider, Contacts, Emails,
    Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/mecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/microsoft-graph/mecheckmembergroups-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://messente.api.gallery.streamdata.io
- type: x-api-stack
  url: http://microsoft.graph.stack.network
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---