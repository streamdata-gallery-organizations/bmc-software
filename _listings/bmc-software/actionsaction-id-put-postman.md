{
  "info": {
    "name": "BMC Software API Update Action",
    "_postman_id": "beea4eae-d6a8-4cd8-b614-39e7de8f2995",
    "description": "Update an existing Action.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "342d56dd-a7b0-4407-8833-9d1d19634a60",
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
              "id": "367cc40a-442e-42d5-a876-c6af59864bd8"
            }
          ]
        },
        {
          "id": "e30a40e2-4ac7-4f0a-9442-3a3627564448",
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
              "id": "399bcb6a-4c2d-4b4d-92e6-ff663af4e810"
            }
          ]
        },
        {
          "id": "aaa23c5d-ecaa-4194-83bd-8a73ecffeb31",
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
              "id": "e4e60a67-6951-4f7b-879e-85e238f9b5fe"
            }
          ]
        },
        {
          "id": "6d1d2973-94e9-41ef-af3d-d266ba1a42c4",
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
              "id": "78cf118c-fc7f-4873-ba00-e283c4e38079"
            }
          ]
        },
        {
          "id": "633b1592-af4c-4b27-ac46-08d761df9627",
          "name": "uninstall-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Uninstalls an action and remove it from the associated alarms(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d373ab5-98a1-4b90-af5c-e049198a0577"
            }
          ]
        },
        {
          "id": "2706c78b-9659-4d84-8f37-63f24fdbeb90",
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
              "id": "06f6bd98-8af5-4ead-942e-5b50d3b95339"
            }
          ]
        },
        {
          "id": "9d0bbeb0-6bf5-466e-80da-fed526693434",
          "name": "get-action",
          "request": {
            "url": "http://example.com/api/v1/actions/:action?action\nName of plugin=action%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d4b14fa-5c9b-45f8-84a8-d69f0a803ddb"
            }
          ]
        },
        {
          "id": "8f5d3cc7-6613-48d8-8ec5-2c60b6609040",
          "name": "create-action",
          "request": {
            "url": "http://example.com/api/actions?action_name\n        \n        \n            required\n            Display name for the Action.\n        \n    \n    \n        \n        action_url\n        \n        \n            required\n            URL to be invoked for action execution.=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d92d38d3-f4c7-4e74-9fb0-60b5d7a82a7f"
            }
          ]
        },
        {
          "id": "3a9e1fc7-13af-4675-b159-2ed01abac873",
          "name": "update-action",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "actions/:action_id"
              ],
              "query": [
                {
                  "key": "action_name\n        \n        \n            required\n            Display name for the Action.\n        \n    \n    \n        \n        action_url\n        \n        \n            required\n            URL to be invoked for action execution.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "action_id",
                  "value": "action_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing Action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cdcf175-9de1-43e5-94e0-c2cd56456572"
            }
          ]
        }
      ]
    }
  ]
}