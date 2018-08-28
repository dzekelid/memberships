{
  "info": {
    "name": "Microsoft Graph API Get Member Objects",
    "_postman_id": "bcae8c0c-849a-474b-897b-434a7b97006e",
    "description": "Get member objects Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "member",
      "item": [
        {
          "id": "b2d3a9e3-4aba-4efe-b261-c2461ab38440",
          "name": "GetMemberObjects",
          "request": {
            "url": "http://graph.microsoft.com/me/getMemberObjects",
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
              "id": "c62f4405-af27-4759-b9bb-8d99966f1ed7"
            }
          ]
        }
      ]
    }
  ]
}