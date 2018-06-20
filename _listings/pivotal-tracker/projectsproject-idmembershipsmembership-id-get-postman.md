{
  "info": {
    "name": "Pivotal Tracker Get Projects Project Memberships Membership",
    "_postman_id": "58400794-5f2f-4e0f-bfea-d1ce27efea0d",
    "description": "Retrieves information about a single membership.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "952c2be1-83b8-4d8c-a4a8-eef02fd31fde",
          "name": "getProjectsProjectMemberships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all memberships for a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddfa4c34-6d19-4387-b41f-7488098fd5f2"
            }
          ]
        },
        {
          "id": "8e8b6810-aff8-4f8e-a7ad-c105516a661b",
          "name": "postProjectsProjectMemberships",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new membership to a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f454ce78-9e52-4624-a593-211e9f242d49"
            }
          ]
        },
        {
          "id": "ad3e204a-70b2-4f53-9fa4-d21bef898679",
          "name": "getProjectsProjectMembershipsMembership",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/memberships/:MEMBERSHIP_ID"
              ],
              "variable": [
                {
                  "id": "MEMBERSHIP_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about a single membership."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "702193aa-fa84-4f7f-b7fd-3a3818eee6fe"
            }
          ]
        }
      ]
    }
  ]
}