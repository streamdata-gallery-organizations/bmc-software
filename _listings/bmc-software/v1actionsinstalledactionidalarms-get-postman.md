{
  "info": {
    "name": "BMC Software API Get all alarms using an action",
    "_postman_id": "77b7744e-3990-4e2a-bc4c-948cd4a2d943",
    "description": "Get alarms that are using this action installed for the project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "fcea9bac-be14-44d6-ab82-f077e5eee937",
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
              "id": "d42175f4-795f-469d-820e-cb2e5d28febe"
            }
          ]
        },
        {
          "id": "d08f3d91-dbee-4e61-ad88-e07d7394cd3e",
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
              "id": "56a695d9-61a3-47bc-8edf-6c0d5abf799d"
            }
          ]
        },
        {
          "id": "601d4d25-443d-4f5e-a969-5a82bf88460e",
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
              "id": "cad48a35-9e18-4758-8dda-a2ba79316467"
            }
          ]
        },
        {
          "id": "3b724da0-6915-4cd3-b0d9-2864f873165a",
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
              "id": "282f3d87-464c-49be-a06d-d1683f2f8aa3"
            }
          ]
        },
        {
          "id": "6b5e1239-2cba-4856-aa39-bf6ec49c7cbd",
          "name": "get-all-alarms-using-an-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get alarms that are using this action installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2433bb8-e47c-4dbf-8947-e199cb7d7bf7"
            }
          ]
        }
      ]
    }
  ]
}