{
  "info": {
    "name": "Microsoft Graph API Get Member Objects",
    "_postman_id": "684ec4a0-1a2f-4e59-892e-ac8de1bfffe6",
    "description": "Get member objects Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "92943066-5e50-400c-a118-9c3bba23c408",
          "name": "GetMemberObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "directoryObjects/:id/getMemberObjects"
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
            "description": "Get member objects Returns all the groups and directory roles that a user, group, or directory object is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "d0d87983-78e9-4592-88b4-1198698dfaa6"
            }
          ]
        }
      ]
    }
  ]
}