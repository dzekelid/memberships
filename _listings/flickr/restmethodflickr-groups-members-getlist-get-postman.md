{
  "info": {
    "name": "Flickr Groups Members Get List",
    "_postman_id": "66e625d2-c45e-498d-b6ee-7deb3f9c76db",
    "description": "Get a list of the members of a group. The call must be signed on behalf of a Flickr member, and the ability to see the group membership will be determined by the Flickr member's group privileges.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "49425204-0bc8-499f-8380-ddce33dd74db",
          "name": "getRestMethodFlickr.groups.browse",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.browse?api_key=%7B%7D&cat_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse the group category tree, finding groups and sub-categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5d9923-c9cd-4a0a-ba62-5551c362c020"
            }
          ]
        },
        {
          "id": "2872d1d8-67e2-4fed-8e80-020b942045df",
          "name": "getRestMethodFlickr.groups.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.getInfo?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "582ad1e2-8488-43b7-8b63-f8ff2beaecd1"
            }
          ]
        },
        {
          "id": "d92e0796-c59d-4a32-a074-948045b7e721",
          "name": "getRestMethodFlickr.groups.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.search?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&text=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28dbcc60-7bc7-4abf-a9c1-9cf80e91646b"
            }
          ]
        },
        {
          "id": "5149411d-d0fa-40b2-bfdc-d1571a0dee0d",
          "name": "getRestMethodFlickr.groups.members.getlist",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.members.getList?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&membertypes=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the members of a group. The call must be signed on behalf of a Flickr member, and the ability to see the group membership will be determined by the Flickr member's group privileges."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f39eff71-1b0c-4c42-8755-953c6cf3be43"
            }
          ]
        }
      ]
    }
  ]
}