{
  "info": {
    "name": "Data.gov API Add Organizations Org Membership",
    "_postman_id": "8b71e421-8784-48ee-8ba8-eb9cf11f1c3e",
    "description": "Apply for membership to a given organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "33d8c8aa-ae88-4a32-9791-30a7c6b33045",
          "name": "postOrganizationsOrgMembership",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:org/membership/"
              ],
              "variable": [
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
            "description": "Apply for membership to a given organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d917a4c4-cf20-4642-838c-097bf3d74918"
            }
          ]
        }
      ]
    }
  ]
}