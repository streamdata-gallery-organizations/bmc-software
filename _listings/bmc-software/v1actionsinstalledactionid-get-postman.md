{
  "info": {
    "name": "BMC Software API Get details of an installed action",
    "_postman_id": "cad39d76-26d8-4595-afd6-43d0230fbab3",
    "description": "Gets a single action definition",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "c4dc7743-d2b7-42a6-9042-e691abfb1aab",
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
              "id": "cd696e1a-185c-4491-b471-870706b6e079"
            }
          ]
        },
        {
          "id": "e6b559f0-3fce-4a75-8194-08027159a89b",
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
              "id": "85464739-e38d-407a-b960-bfb2628e8881"
            }
          ]
        },
        {
          "id": "3cc82aba-9191-4858-af92-1b1688ec241f",
          "name": "install-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an action"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1514fd6c-3b48-407b-bf01-58b5785994b1"
            }
          ]
        },
        {
          "id": "5bb5a639-a0c0-4ff8-9848-eb42aa67610e",
          "name": "get-details-of-an-installed-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId?actionId\nName of plugin=actionId%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0556aa26-5ceb-4c78-a4a7-09ca0ca165ad"
            }
          ]
        }
      ]
    }
  ]
}