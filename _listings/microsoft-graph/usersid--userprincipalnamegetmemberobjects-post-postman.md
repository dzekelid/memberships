{
  "info": {
    "name": "Microsoft Graph API Get Member Objects",
    "_postman_id": "d8458770-c63a-4cbb-98c6-4f15ed72eab4",
    "description": "Get member objects Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "540c392d-f009-4b8a-9c46-b435dd148827",
          "name": "GetMemberObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/getMemberObjects"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get member objects Returns all the groups and directory roles that a user, group, or directory object is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "1df18205-faa4-4b64-80e1-3b0d5471a566"
            }
          ]
        }
      ]
    }
  ]
}