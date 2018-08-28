---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Edit Group Members
  description: |-
    Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/groups/{groupId}/bulk-assign:
    post:
      summary: Edit Group Members
      description: |-
        Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: assignGlipGroupMembers
      x-api-path-slug: restapiv1-0glipgroupsgroupidbulkassign-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Group
      - Members
  /restapi/v1.0/account/{accountId}/department/bulk-assign:
    post:
      summary: Edit Call Queue Members
      description: "[Deprecated] Adds and/or removes multiple call queue members\nApp
        Permission\nEditAccounts\nUser Permission\nUserGroups\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nEXT-401\nExtension
        ID should be present only in one section"
      operationId: bulkAssignDepartments
      x-api-path-slug: restapiv1-0accountaccountiddepartmentbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Call
      - Queue
      - Members
  /restapi/v1.0/account/{accountId}/call-queues/{groupId}/members:
    get:
      summary: Get Call Queue Members
      description: |-
        Returns call queue group members.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Light
      operationId: listCallQueueMembers
      x-api-path-slug: restapiv1-0accountaccountidcallqueuesgroupidmembers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: groupId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Queue
      - Members
  /restapi/v1.0/account/{accountId}/call-monitoring-groups/{groupId}/members:
    get:
      summary: Get Call Monitoring Group Members
      description: |-
        Returns call monitoring group members.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallMonitoringGroupMembers
      x-api-path-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: groupId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Monitoring
      - Group
      - Members
  /restapi/v1.0/account/{accountId}/department/{departmentId}/members:
    get:
      summary: Get Department Member List
      description: "[Deprecated] Viewing user account info (including name, business
        name, address and phone number/account number)\nApp Permission\nReadAccounts\nUser
        Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
        for parameter [departmentId] is not found"
      operationId: listDepartmentMembers
      x-api-path-slug: restapiv1-0accountaccountiddepartmentdepartmentidmembers-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: departmentId
        description: Internal identifier of a Department extension (same as extensionId
          but only the ID of a department extension is valid)
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Department
      - Member
      - List
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