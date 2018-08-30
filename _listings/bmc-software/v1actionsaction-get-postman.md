{
  "info": {
    "name": "BMC Software API Get action",
    "_postman_id": "2315599c-dbef-4fc3-b8c3-3321e71fcef0",
    "description": "Gets a single action type",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "ad929098-6e55-485d-9b07-6f667cd39e70",
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
              "id": "c2419b7d-f47a-451b-a5ab-caff84c3189d"
            }
          ]
        },
        {
          "id": "7856ba91-d634-42e2-b9ad-8eb1299b3182",
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
              "id": "505a5d32-a3f3-4f24-b427-f71554871247"
            }
          ]
        },
        {
          "id": "f285cd31-c38c-4dd8-a449-7f0355e38906",
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
              "id": "d5a5a203-24f1-448f-8146-415c3fe72872"
            }
          ]
        },
        {
          "id": "c524aa3f-0982-4be9-86ee-70bcdb25c3eb",
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
              "id": "12165b4d-2b43-47ef-933b-1fd0986d02df"
            }
          ]
        },
        {
          "id": "c0fc0710-b31e-48c7-8023-43d79f20f982",
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
              "id": "5e70bc0c-6194-4104-829c-1c2444c8951e"
            }
          ]
        },
        {
          "id": "f6ce4a8c-6666-4863-a551-0b9e3457be5a",
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
              "id": "b881c5a1-64df-4f27-801b-404724d414f0"
            }
          ]
        },
        {
          "id": "b3c5b253-aa51-4a23-aa68-ec6b9c68d3e9",
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
              "id": "260b6726-7d27-4922-87f4-9e3e11790798"
            }
          ]
        }
      ]
    }
  ]
}