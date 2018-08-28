{
  "info": {
    "name": "Microsoft Graph API Check Member Groups",
    "_postman_id": "979aecce-f18f-45b0-99d3-e00c6859b13d",
    "description": "Check member groups Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "checks",
      "item": [
        {
          "id": "9b5e06cd-baf6-4610-acbf-4a7e99c40e87",
          "name": "CheckMemberGroups",
          "request": {
            "url": "http://graph.microsoft.com/me/checkMemberGroups",
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
              "id": "f0345e6f-aa57-433e-8b40-5f5781e1856f"
            }
          ]
        }
      ]
    }
  ]
}