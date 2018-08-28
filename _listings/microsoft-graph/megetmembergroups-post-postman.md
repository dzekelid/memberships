{
  "info": {
    "name": "Microsoft Graph API Get Member Groups",
    "_postman_id": "3597fae0-01fe-4237-8a2c-a78a25ebd51b",
    "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "f5ee26d5-18e4-4ea3-83b8-872db56115b7",
          "name": "GetMemberGroups",
          "request": {
            "url": "http://graph.microsoft.com/me/getMemberGroups",
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
            "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "00fc5d65-7868-4cfa-a98f-82454a8a2ad2"
            }
          ]
        }
      ]
    }
  ]
}