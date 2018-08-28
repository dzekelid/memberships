{
  "info": {
    "name": "Microsoft Graph API Check Member Groups",
    "_postman_id": "67a456dc-a870-41d0-9bb8-f8b5b64f9b21",
    "description": "Check member groups Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "checks",
      "item": [
        {
          "id": "9a717f4a-055c-4e9b-b9df-1f37d5704571",
          "name": "CheckMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "directoryObjects/:id/checkMemberGroups"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
              "id": "600a975b-0226-43cc-a50b-b0ce1b9582b0"
            }
          ]
        }
      ]
    }
  ]
}