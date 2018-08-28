{
  "info": {
    "name": "Microsoft Graph API Group Check Member Groups",
    "_postman_id": "c4de6a1d-8078-4794-80db-e75eb76b702a",
    "description": "group: checkMemberGroups Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group",
      "item": [
        {
          "id": "a27a5dca-5868-4e9a-a223-bc1dc498a672",
          "name": "Group:CheckMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/checkMemberGroups"
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
            "description": "group: checkMemberGroups Check for membership in the specified list of groups"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "420f0c49-0d5c-4730-815d-41b6f6aa0baf"
            }
          ]
        }
      ]
    }
  ]
}