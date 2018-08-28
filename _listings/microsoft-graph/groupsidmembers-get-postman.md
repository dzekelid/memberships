{
  "info": {
    "name": "Microsoft Graph API List Members",
    "_postman_id": "0d7bba13-ae7f-4b4d-b46f-faffdf77ec2b",
    "description": "List members Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "2d7963e7-fc43-4c15-bcbd-55f39c3a0b7b",
          "name": "ListMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/members"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List members Get a list of the group's direct members"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a8921a3c-b3e2-4761-840e-33ca496041db"
            }
          ]
        }
      ]
    }
  ]
}