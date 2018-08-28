{
  "info": {
    "name": "Twilio Delete Queue Members",
    "_postman_id": "5687237d-71b8-4a9a-b71c-8503fd88f4a7",
    "description": "The DELETE method allows you to remove a Queue. Only empty queues arendeletable.n",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "queues",
      "item": [
        {
          "id": "58cdee43-3098-49f0-9463-cd57ea8b11ce",
          "name": "the-delete-method-allows-you-to-remove-a-queue-only-empty-queues-aredeletable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Queues/:QueueSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "QueueSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "The DELETE method allows you to remove a Queue"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"queue\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "44f7226b-0191-4366-bfda-edb7de3bf932"
            }
          ]
        }
      ]
    }
  ]
}