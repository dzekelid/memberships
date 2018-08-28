{
  "info": {
    "name": "Microsoft Graph API Check Member Groups",
    "_postman_id": "e8b46029-b720-415d-bbc4-4ba4f5aa6867",
    "description": "Check member groups Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "checks",
      "item": [
        {
          "id": "046e4e30-58f1-4ce2-bb7b-263e5bfc4375",
          "name": "CheckMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/checkMemberGroups"
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
            "description": "Check member groups Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "0bbf2fb4-57fb-47c5-8502-e7673836fdb2"
            }
          ]
        }
      ]
    }
  ]
}