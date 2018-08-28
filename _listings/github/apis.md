---
name: GitHub
x-slug: github
description: GitHub brings together the worlds largest community of developers to
  discover, share, and build better software. From open source projects to private
  team repositories, were your all-in-one platform for collaborative development.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
x-kinRank: "10"
x-alexaRank: "64"
tags: Memberships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/apis.md
specificationVersion: "0.14"
apis:
- name: GitHub - Delete Teams Team Memberships Username
  x-api-slug: teamsteamidmembershipsusername-delete
  description: |-
    Remove team membership.
    In order to remove a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with. NOTE: This does not delete the user, it just removes their membership from the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-delete-openapi.md
- name: GitHub - Get Teams Team Memberships Username
  x-api-slug: teamsteamidmembershipsusername-get
  description: |-
    Get team membership.
    In order to get a user's membership with a team, the authenticated user must be a member of the team or an owner of the team's organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-get-openapi.md
- name: GitHub - Put Teams Team Memberships Username
  x-api-slug: teamsteamidmembershipsusername-put
  description: |-
    Add team membership.
    In order to add a membership between a user and a team, the authenticated user must have 'admin' permissions to the team or be an owner of the organization that the team is associated with.

    If the user is already a part of the team's organization (meaning they're on at least one other team in the organization), this endpoint will add the user to the team.

    If the user is completely unaffiliated with the team's organization (meaning they're on none of the organization's teams), this endpoint will send an invitation to the user via email. This newly-created membership will be in the 'pending' state until the user accepts the invitation, at which point the membership will transition to the 'active' state and the user will be added as a member of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembershipsusername-put-openapi.md
- name: GitHub - Get Orgs Org Members
  x-api-slug: orgsorgmembers-get
  description: |-
    Members list.
    List all users who are members of an organization. A member is a user tha
    belongs to at least 1 team in the organization. If the authenticated user
    is also an owner of this organization then both concealed and public members
    will be returned. If the requester is not an owner of the organization the
    query will be redirected to the public members list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembers-get-openapi.md
- name: GitHub - Delete Orgs Org Members Username
  x-api-slug: orgsorgmembersusername-delete
  description: |-
    Remove a member.
    Removing a user from this list will remove them from all teams and they
    will no longer have any access to the organization's repositories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-delete-openapi.md
- name: GitHub - Get Orgs Org Members Username
  x-api-slug: orgsorgmembersusername-get
  description: Check if a user is, publicly or privately, a member of the organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-get-openapi.md
- name: GitHub - Get Orgs Org Public Members
  x-api-slug: orgsorgpublic-members-get
  description: |-
    Public members list.
    Members of an organization can choose to have their membership publicized
    or not.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-members-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-members-get-openapi.md
- name: GitHub - Delete Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-delete
  description: Conceal a user's membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-delete-openapi.md
- name: GitHub - Get Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-get
  description: Check public membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-get-openapi.md
- name: GitHub - Put Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-put
  description: Publicize a user's membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-put-openapi.md
- name: GitHub - Get Teams Team Members
  x-api-slug: teamsteamidmembers-get
  description: |-
    List team members.
    In order to list members in a team, the authenticated user must be a member
    of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembers-get-openapi.md
- name: GitHub - Delete Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-delete
  description: |-
    The "Remove team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Remove team membership API instead. It allows you to remove both active and pending memberships.

    Remove team member.
    In order to remove a user from a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
    NOTE This does not delete the user, it just remove them from the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-delete-openapi.md
- name: GitHub - Get Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-get
  description: |-
    The "Get team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Get team membership API instead. It allows you to get both active and pending memberships.

    Get team member.
    In order to get if a user is a member of a team, the authenticated user mus
    be a member of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-get-openapi.md
- name: GitHub - Put Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-put
  description: |-
    The API (described below) is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Add team membership API instead. It allows you to invite new organization members to your teams.

    Add team member.
    In order to add a user to a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-put-openapi.md
- name: GitHub - Put Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-put
  description: |-
    The API (described below) is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Add team membership API instead. It allows you to invite new organization members to your teams.

    Add team member.
    In order to add a user to a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-put-openapi.md
- name: GitHub - Get Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-get
  description: |-
    The "Get team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Get team membership API instead. It allows you to get both active and pending memberships.

    Get team member.
    In order to get if a user is a member of a team, the authenticated user mus
    be a member of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-get-openapi.md
- name: GitHub - Delete Teams Team Members Username
  x-api-slug: teamsteamidmembersusername-delete
  description: |-
    The "Remove team member" API is deprecated and is scheduled for removal in the next major version of the API. We recommend using the Remove team membership API instead. It allows you to remove both active and pending memberships.

    Remove team member.
    In order to remove a user from a team, the authenticated user must have 'admin'
    permissions to the team or be an owner of the org that the team is associated
    with.
    NOTE This does not delete the user, it just remove them from the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembersusername-delete-openapi.md
- name: GitHub - Get Teams Team Members
  x-api-slug: teamsteamidmembers-get
  description: |-
    List team members.
    In order to list members in a team, the authenticated user must be a member
    of the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/teamsteamidmembers-get-openapi.md
- name: GitHub - Put Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-put
  description: Publicize a user's membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-put-openapi.md
- name: GitHub - Get Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-get
  description: Check public membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-get-openapi.md
- name: GitHub - Delete Orgs Org Public Members Username
  x-api-slug: orgsorgpublic-membersusername-delete
  description: Conceal a user's membership.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-membersusername-delete-openapi.md
- name: GitHub - Get Orgs Org Public Members
  x-api-slug: orgsorgpublic-members-get
  description: |-
    Public members list.
    Members of an organization can choose to have their membership publicized
    or not.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-members-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgpublic-members-get-openapi.md
- name: GitHub - Get Orgs Org Members Username
  x-api-slug: orgsorgmembersusername-get
  description: Check if a user is, publicly or privately, a member of the organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-get-openapi.md
- name: GitHub - Delete Orgs Org Members Username
  x-api-slug: orgsorgmembersusername-delete
  description: |-
    Remove a member.
    Removing a user from this list will remove them from all teams and they
    will no longer have any access to the organization's repositories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembersusername-delete-openapi.md
- name: GitHub - Get Orgs Org Members
  x-api-slug: orgsorgmembers-get
  description: |-
    Members list.
    List all users who are members of an organization. A member is a user tha
    belongs to at least 1 team in the organization. If the authenticated user
    is also an owner of this organization then both concealed and public members
    will be returned. If the requester is not an owner of the organization the
    query will be redirected to the public members list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/github-logo.png
  humanURL: https://github.com
  baseURL: https://api.github.com//
  tags: Social, Coding, Programming, Social, Jobs, Hacker Storytelling, Code, My API
    Stack, Management, Imports, Issues, Issue Management, Change Log Example, Stack
    Network, Stack, SaaS, Technology, Developers, API Provider, API Service Provider,
    Profiles, General Data, Relative Data, Pedestal, Historical Data API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/memberships/master/_listings/github/orgsorgmembers-get-openapi.md
x-common:
- type: x--net-library
  url: https://github.com/octokit/octokit.net
- type: x-api-gallery
  url: http://giphy.api.gallery.streamdata.io
- type: x-api-stack
  url: http://github.stack.network
- type: x-base
  url: https://api.github.com
- type: x-blog
  url: http://github.com/blog
- type: x-blog-rss
  url: https://github.com/blog/subscribe
- type: x-change-log
  url: https://developer.github.com/changes/
- type: x-contact-form
  url: https://github.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/github
- type: x-crunchbase
  url: https://crunchbase.com/organization/github
- type: x-developer
  url: https://developer.github.com/
- type: x-github
  url: https://github.com/github
- type: x-guides
  url: https://developer.github.com/guides/
- type: x-ios-sdk
  url: https://github.com/octokit/octokit.objc
- type: x-pricing
  url: https://github.com/pricing
- type: x-privacy
  url: http://help.github.com/privacy-policy/
- type: x-ruby-library
  url: https://github.com/octokit/octokit.rb
- type: x-security
  url: http://help.github.com/security/
- type: x-status
  url: https://status.github.com/
- type: x-terms-of-service
  url: http://help.github.com/terms-of-service/
- type: x-transparency-report
  url: https://github.com/blog/1987-github-s-2014-transparency-report
- type: x-twitter
  url: https://twitter.com/github
- type: x-webhooks
  url: https://developer.github.com/webhooks/
- type: x-website
  url: https://github.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---