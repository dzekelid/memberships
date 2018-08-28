{
  "info": {
    "name": "Microsoft Graph API Group Get Member Objects",
    "_postman_id": "9ab856ef-65bf-408d-914c-a9087df6fc8f",
    "description": "group: getMemberObjects Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "group",
      "item": [
        {
          "id": "df82b886-aef8-4b41-9db5-8039a01319a4",
          "name": "Group:GetMemberObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/getMemberObjects"
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
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "group: getMemberObjects Return all of the groups that this group is a member of"
          },
          "response": [
            {
              "status": "Successful Response",
              "code": 200,
              "name": "Response_200",
              "id": "a8255163-34f7-45fe-ba9b-78a52e835d9a"
            }
          ]
        }
      ]
    }
  ]
}