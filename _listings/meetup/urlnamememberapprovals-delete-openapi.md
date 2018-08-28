---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Membership Decline
  description: Declines one or more requests for group membership
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/member/approvals:
    post:
      summary: Membership Approval
      description: Approves one or more requests for group membership
      operationId: profiles
      x-api-path-slug: urlnamememberapprovals-post
      parameters:
      - in: query
        name: member
        description: Comma-delimited numeric pending member IDs
        type: string
      - in: query
        name: send_copy
        description: Optional boolean value indicating whether or not the org should
          receive a copy of the message sent to the approved members
        type: string
      - in: query
        name: welcome_message
        description: Optional message to send to the members being approved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
    delete:
      summary: Membership Decline
      description: Declines one or more requests for group membership
      operationId: profiles
      x-api-path-slug: urlnamememberapprovals-delete
      parameters:
      - in: query
        name: anon
        description: Optional Boolean value indicating whether the declining members
          email address should be hidden in the resulting response
        type: string
      - in: query
        name: ban
        description: Optional Boolean value indicating whether or not to ban the member
          in the future
        type: string
      - in: query
        name: explanation
        description: Optional explanation to send to the members being declined
        type: string
      - in: query
        name: member
        description: Comma-delimited numeric pending member IDs
        type: string
      - in: query
        name: send_copy
        description: Optional Boolean value indicating whether or not to send a copy
          to the member issuing the decline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
  /members:
    get:
      summary: Members
      description: API method for accessing members of Meetup Groups
      operationId: deprecated
      x-api-path-slug: members-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_id
        description: Return members in groups with these ID numbers, separated by
          commas
        type: string
      - in: query
        name: group_urlname
        description: Return members for the group with the given custom URL path
        type: string
      - in: query
        name: member_id
        description: Return the member with this ID
        type: string
      - in: query
        name: relation
        description: Supply the string self as the value for this parameter to get
          the information of the member linked to the API key making the request
        type: string
      - in: query
        name: service
        description: Match users by the external services theyve linked to their member
          account, specified as servicename:identifier
        type: string
      - in: query
        name: topic,groupnum
        description: Return members for the group with given topic and number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Members
  /self/blocks/:member_id:
    post:
      summary: Block member
      description: Blocks a target member from various interactions with the authenticated
        member on the platform
      operationId: abuse
      x-api-path-slug: selfblocksmember-id-post
      parameters:
      - in: query
        name: comments
        description: An optional string of text describing why you have chosen to
          block this member
        type: string
      - in: query
        name: report
        description: An optional value that represents a type of abuse the target
          member is being blocked for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Abuse
      - Members
    delete:
      summary: Unblock member
      description: Unblocks a previously blocked member from various interactions
        with the authenticated member on the platform
      operationId: abuse
      x-api-path-slug: selfblocksmember-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Abuse
      - Members
  /self/events:
    get:
      summary: Member Events
      description: |-
        Gets a listing of all scheduled Meetup Events the authenticated member has RSVP'd to
        that have been announced to the group.
        This listing is ordered from oldest to most recent by default
      operationId: events
      x-api-path-slug: selfevents-get
      parameters:
      - in: query
        name: desc
        description: When true, sorts results in descending order
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional fields names which may be
          appended to the response
        type: string
      - in: query
        name: page
        description: Number of results to return
        type: string
      - in: query
        name: rsvp
        description: Comma-delimited list of RSVP responses
        type: string
      - in: query
        name: scroll
        description: A string representing an alias for a point on a timeline
        type: string
      - in: query
        name: status
        description: Comma-delimited list of event statuses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
  /self/calendar:
    get:
      summary: Member Calendar
      description: Get a listing of all upcoming Meetup events for the authenticated
        member
      operationId: events
      x-api-path-slug: selfcalendar-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields names which may be
          appended to the response
        type: string
      - in: query
        name: page
        description: Number of results to return in a page
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
      - Calendardars
  /self/groups:
    get:
      summary: Member groups
      description: |-
        Lists the authenticated member's groups in the order of leadership,
        next upcoming event, then alphabetical order by name
      operationId: groups
      x-api-path-slug: selfgroups-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: page
        description: Number of groups to return in a single page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
      - Groups
  /2/members:
    get:
      summary: Members
      description: API method for accessing members of Meetup Groups
      operationId: members
      x-api-path-slug: 2members-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_id
        description: Return members in groups with these ID numbers, separated by
          commas
        type: string
      - in: query
        name: group_urlname
        description: Return members for the group with the given custom URL path
        type: string
      - in: query
        name: member_id
        description: Return the member with this ID
        type: string
      - in: query
        name: service
        description: Match users by the external services theyve linked to their member
          account, specified as servicename:identifier
        type: string
      - in: query
        name: topic,groupnum
        description: Return members for the group with given topic and number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/member/:id:
    get:
      summary: Member Get
      description: Retrieve a single member
      operationId: members
      x-api-path-slug: 2memberid-get
      parameters:
      - in: query
        name: fields
        description: comma-separate list of optional fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
    post:
      summary: Member Edit
      description: Edit the authorized member's attributes
      operationId: members
      x-api-path-slug: 2memberid-post
      parameters:
      - in: query
        name: add_topics
        description: Comma-delimited list of topics ids to add to your alert list
        type: string
      - in: query
        name: bio
        description: Free form text passage about you
        type: string
      - in: query
        name: bio_privacy
        description: Controls the visibility of the members bio
        type: string
      - in: query
        name: birthday
        description: Day you were born
        type: string
      - in: query
        name: city
        description: City name for your location
        type: string
      - in: query
        name: city_id
        description: Valid city id from /2/cities method
        type: string
      - in: query
        name: country
        description: Valid country code for your location
        type: string
      - in: query
        name: facebook_privacy
        description: Controls the visibility of the members facebook connection
        type: string
      - in: query
        name: gender
        description: Your gender (used for better recommendations)
        type: string
      - in: query
        name: groups_privacy
        description: Controls the visibility of the members groups
        type: string
      - in: query
        name: hometown
        description: Hometown of member
        type: string
      - in: query
        name: lang
        description: Language preference used on the site
        type: string
      - in: query
        name: lat
        description: latitude of city
        type: string
      - in: query
        name: lon
        description: longitude of city
        type: string
      - in: query
        name: messaging_pref
        description: This specifies the members preference for being contacted from
          members on the site
        type: string
      - in: query
        name: name
        description: The name of the current member
        type: string
      - in: query
        name: photos_privacy
        description: Controls the visibility of the members photos
        type: string
      - in: query
        name: photo_id
        description: A valid photo_id from the members photos to set as the main profile
          photo
        type: string
      - in: query
        name: radius
        description: radius, in miles to search for city given a lat and lon
        type: string
      - in: query
        name: remove_topics
        description: Comma-delimited list of topic ids to remove from your alert list
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      - in: query
        name: topics_privacy
        description: Controls the visibility of the members topics
        type: string
      - in: query
        name: zip
        description: Valid zip code for city
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/member_photo:
    post:
      summary: Member Photo Upload
      description: Uploads a photo to be associated with a Member
      operationId: members
      x-api-path-slug: 2member-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the members main profile
          photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: sync_matching_photo
        description: When set to true and main is set to true, this will replace all
          group profile photos matching the current photo with the provided replacement
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/member_photo/:id:
    delete:
      summary: Member Photo Delete
      description: Delete the specified member photo
      operationId: members
      x-api-path-slug: 2member-photoid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
  /:urlname/members/:member_id:
    get:
      summary: Get Group Member Profile
      description: |-
        Gets Group Profiles.
        For Member Profiles, see [this endpoint](/meetup_api/docs/members/:member_id)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    patch:
      summary: Edit Group Member Profile
      description: |-
        Edits Group Profiles.
        To fetch Group Member Profiles,
        see [this endpoint](/meetup_api/docs/:urlname/members/:member_id#get)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-patch
      parameters:
      - in: query
        name: add_role
        description: Allows those with permission to assign one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: answer_{qid}
        description: Answers to questions from groups API join_info question fields
        type: string
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      - in: query
        name: intro
        description: Provides a Member an opportunity to tell the group about themselves,in
          at most 255 characters
        type: string
      - in: query
        name: photo_id
        description: Numeric id of the photo to use for this profile
        type: string
      - in: query
        name: remove_role
        description: Allows those with permission to remove one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: title
        description: An organizer-defined title,in at most 255 characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    delete:
      summary: Delete Group Member Profile (Leave Group)
      description: Deletes a member's group profiles.
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-delete
      parameters:
      - in: query
        name: exit_comment
        description: Optional message to the organizer when leaving
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---