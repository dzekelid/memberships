{
  "info": {
    "name": "Microsoft Graph API Group Get Member Groups",
    "_postman_id": "521d2247-7fa7-4588-9d1c-2f731cef7f3d",
    "description": "group: getMemberGroups Return all the groups that the specified group is a member of. The check is transitive, unlike reading the memberOf navigation property, which returns only the groups that the group is a direct member of.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group",
      "item": [
        {
          "id": "376d059e-9254-44e9-9b02-d3a9f2a80cf1",
          "name": "Group:GetMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/getMemberGroups"
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
            "description": "group: getMemberGroups Return all the groups that the specified group is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "34a0e772-9ab4-44ed-82fb-3b6fff67be85"
            }
          ]
        }
      ]
    }
  ]
}