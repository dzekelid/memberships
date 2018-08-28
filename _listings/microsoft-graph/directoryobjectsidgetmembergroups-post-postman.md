{
  "info": {
    "name": "Microsoft Graph API Get Member Groups",
    "_postman_id": "d67dff99-6de5-409b-ba80-32572e5d0b80",
    "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "778bf5c9-37d5-4cb7-bd75-c5e576dfb604",
          "name": "GetMemberGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "directoryObjects/:id/getMemberGroups"
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
            "description": "Get member groups Return all the groups that the specified user, group, or directory object is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "a862870c-e588-4463-b501-7bb1e6a00319"
            }
          ]
        }
      ]
    }
  ]
}