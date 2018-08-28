{
  "info": {
    "name": "Data.gov API Add Organizations Org Membership  Accept",
    "_postman_id": "78a58c98-20a1-4ea0-8d77-fd26d424c9d7",
    "description": "Accept user membership to a given organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "9ee78b09-34bd-4bb2-9639-5ddfb0301a44",
          "name": "postOrganizationsOrgMembershipAccept",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:org/membership/:id/accept/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "org",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Accept user membership to a given organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41dca335-7fed-4a1a-bf42-69a2f744ff8f"
            }
          ]
        }
      ]
    }
  ]
}