{
  "info": {
    "name": "Microsoft Graph API Get Member Groups",
    "_postman_id": "eaebe2e5-edda-40f1-9383-dcca15632c3b",
    "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "734fcfd7-9418-4323-a92c-cd6c771db0a6",
          "name": "GetMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/getMemberGroups"
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
            "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "7673b688-20ea-4ace-b54c-bade5d6840c5"
            }
          ]
        }
      ]
    }
  ]
}