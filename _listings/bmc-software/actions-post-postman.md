{
  "info": {
    "name": "BMC Software API Create Action",
    "_postman_id": "35c955f7-70a1-4949-a1f7-4dad5f5777ad",
    "description": "Create a new Action.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "cfcb45a1-9b10-4899-81ba-1437a205aa95",
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
              "id": "bd9d5c49-06db-474b-a1cb-b2ce8c8ecdeb"
            }
          ]
        },
        {
          "id": "711e1e07-4757-4049-a9e4-c7cb0ddf0068",
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
              "id": "b23dba9a-79b5-49c6-8cda-012568353a3d"
            }
          ]
        },
        {
          "id": "06c75e54-ca9e-4e19-a68e-f3e3c3b1bd80",
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
              "id": "c8f0b276-4e9f-441e-8d6c-c057b592ae07"
            }
          ]
        },
        {
          "id": "0e2a072a-dcd8-41cb-b19a-f9635a5e5381",
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
              "id": "a7a96c62-4ed3-4112-92c1-4049b8cca1ec"
            }
          ]
        },
        {
          "id": "46cdf8d6-0ea3-43c2-9750-1303158aa877",
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
              "id": "a73e4c48-6ab2-4971-b474-e28f7c7f4dbf"
            }
          ]
        },
        {
          "id": "f691bdb3-207e-4cd1-8c0d-73d87f33c47b",
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
              "id": "37b9c3dc-27f8-4439-bcec-63bc565b2be2"
            }
          ]
        },
        {
          "id": "65f78400-0f58-4efa-98f9-d7c396b886e9",
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
              "id": "b0521789-bd8d-4cf2-9a15-90c854eca645"
            }
          ]
        },
        {
          "id": "2db864ce-772e-4734-8ea6-6d3ad89a98c5",
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
              "id": "476c2038-426c-44ed-a23f-9de1de267aa5"
            }
          ]
        }
      ]
    }
  ]
}