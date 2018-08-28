{
  "info": {
    "name": "Data.gov API Delete Organizations Org Member User",
    "_postman_id": "11dc7342-8d0d-4f5f-b71e-12deec4f12f4",
    "description": "Delete member from an organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "be370c41-bed5-4b09-96b6-72591c1bed4d",
          "name": "deleteOrganizationsOrgMemberUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:org/member/:user"
              ],
              "variable": [
                {
                  "id": "org",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete member from an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b57f36b-66e6-4037-bebe-af155e0b3ddd"
            }
          ]
        }
      ]
    }
  ]
}