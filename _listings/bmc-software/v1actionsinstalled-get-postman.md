{
  "info": {
    "name": "BMC Software API Get all installed actions",
    "_postman_id": "a5c99d0c-6dd1-4f95-97f4-11706d3cfb3b",
    "description": "Gets all actions that are installed for the project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "81774af9-2879-493e-aed6-d9678bb4b919",
          "name": "get-all-available-action-types",
          "request": {
            "url": "http://example.com/api/v1/actions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all known action types"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ef992b3-9ce7-4f4a-bf82-60af68dcf887"
            }
          ]
        },
        {
          "id": "a7b8bdc5-49a4-4850-90cb-8591193ce74e",
          "name": "get-all-installed-actions",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all actions that are installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "226c973c-1cd9-45dd-b672-679725f99dc6"
            }
          ]
        }
      ]
    }
  ]
}