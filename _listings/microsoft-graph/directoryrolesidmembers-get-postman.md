{
  "info": {
    "name": "Microsoft Graph API List Members",
    "_postman_id": "c28ddbde-1a37-48ba-976d-76104e9a5b6e",
    "description": "List members Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "3ad0fda2-1b94-4149-8caa-a23556bce405",
          "name": "ListMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "directoryRoles/:id/members"
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
            "description": "List members Retrieve a list of the users that are assigned to the directory role"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d62e3422-4921-407e-8813-2a34cf02640d"
            }
          ]
        }
      ]
    }
  ]
}