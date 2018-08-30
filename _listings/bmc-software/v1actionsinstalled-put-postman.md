{
  "info": {
    "name": "BMC Software API Install action",
    "_postman_id": "ca45a056-1434-4bb2-b98b-735546be6cac",
    "description": "Installs an action",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "03e93bc0-dc16-43a6-a08c-341ad333e356",
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
              "id": "31913688-1a40-4ffe-9560-4ba5ad0b3272"
            }
          ]
        },
        {
          "id": "15d826ad-50c1-4469-9bcb-9448ee4428b7",
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
              "id": "41c98b0e-a6c1-49c8-9b83-998b7de89bb9"
            }
          ]
        },
        {
          "id": "4d324d4f-22f8-43bc-bbfe-380e969de92d",
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
              "id": "0fa68fb6-018b-4b4b-b4fc-bc1e1312ef32"
            }
          ]
        }
      ]
    }
  ]
}