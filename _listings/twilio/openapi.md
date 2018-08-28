swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Queues/{QueueSid}:
    delete:
      summary: Delete Queue Members
      description: The DELETE method allows you to remove a Queue. Only empty queues
        arendeletable.n
      operationId: the-delete-method-allows-you-to-remove-a-queue-only-empty-queues-aredeletable
      x-api-path-slug: accountsaccountsidqueuesqueuesid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
    get:
      summary: Get Queue Members
      description: Get resources individual Queue instance.n
      operationId: get-resources-individual-queue-instance
      x-api-path-slug: accountsaccountsidqueuesqueuesid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
    post:
      summary: Add Queue Members
      description: This POST request allows you to change the FriendlyName or MaxSize.n
      operationId: this-post-request-allows-you-to-change-the-friendlyname-or-maxsize
      x-api-path-slug: accountsaccountsidqueuesqueuesid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
  /Accounts/{AccountSid}/Queues/{QueueSid}/Members:
    get:
      summary: Get Queue Members
      description: Returns the list of members in the queue identified by {QueueSid}.
      operationId: returns-the-list-of-members-in-the-queue-identified-by-queuesid
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembers-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
  /Accounts/{AccountSid}/Queues/{QueueSid}/Members/Front:
    get:
      summary: Get Queue Members In Front
      description: Get a front member.
      operationId: get-a-front-member
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembersfront-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
    post:
      summary: Update Queue Members In Front
      description: Posting a URL and Method to a Queue instance will dequeue a member
        from anqueue and have the members call begin executing the TwiML document
        at that URLnWhen dequeuing the Front of the queue, the next call in the queue
        will be redirected.n
      operationId: posting-a-url-and-method-to-a-queue-instance-will-dequeue-a-member-from-aqueue-and-have-the-members-
      x-api-path-slug: accountsaccountsidqueuesqueuesidmembersfront-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
  /Accounts/{AccountSid}/Queues/{QueueSid}/Members/{CallSid}:
    get:
      summary: Get Queue Members
      description: Get a specific member.
      operationId: get-a-specific-member
      x-api-path-slug: accountsaccountsidqueuesqueuesidmemberscallsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CallSid
        description: A 34 character string that uniquely identifies the call
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues
    post:
      summary: Update Queue Members
      description: Posting a URL and Method to a Queue instance will dequeue a member
        from anqueue and have the members call begin executing the TwiML document
        at that URLnWhen redirecting a member of a queue addressed by CallSid, only
        the first requestnwill succeed and return a 200 response code. A second request
        will fail andnreturn an appropriate 400 response code.n
      operationId: posting-a-url-and-method-to-a-queue-instance-will-dequeue-a-member-from-aqueue-and-have-the-members-
      x-api-path-slug: accountsaccountsidqueuesqueuesidmemberscallsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CallSid
        description: A 34 character string that uniquely identifies the call
      - in: path
        name: QueueSid
        description: A 34 character string that uniquely identifies the queue
      responses:
        200:
          description: OK
      tags:
      - Queues