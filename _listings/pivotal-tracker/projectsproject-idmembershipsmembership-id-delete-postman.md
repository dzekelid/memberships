{
  "info": {
    "name": "Pivotal Tracker Delete Projects Project Memberships Membership",
    "_postman_id": "31c3cebb-fed4-426a-80d7-9e576a1d8304",
    "description": "Delete projects project memberships membership.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "05892c40-2cb9-49ec-b44a-7d3994a93019",
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
              "id": "2b242e26-45e8-4afa-9119-4910e8434029"
            }
          ]
        },
        {
          "id": "7f15a145-3ac6-4943-914f-b0636c44c62a",
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
              "id": "b3c89f38-c378-4008-8e7c-e783ac56fb09"
            }
          ]
        },
        {
          "id": "f799df05-10df-459f-9c07-842b6ee09e67",
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
              "id": "8f8abe2d-6810-4769-a72f-2485ccb45fa9"
            }
          ]
        },
        {
          "id": "c0a7c973-f3bb-4458-8442-f66d8309c6b5",
          "name": "deleteProjectsProjectMembershipsMembership",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete projects project memberships membership."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a80b573e-1a46-4dec-91fc-a84c53f23895"
            }
          ]
        }
      ]
    }
  ]
}