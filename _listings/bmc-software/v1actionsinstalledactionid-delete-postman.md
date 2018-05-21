{
  "info": {
    "name": "BMC Software API Uninstall action",
    "_postman_id": "1377e848-43f4-443c-af17-87e871e7e71a",
    "description": "Uninstalls an action and remove it from the associated alarms(s).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "e03f1a01-0233-4538-9879-647714ae553c",
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
              "id": "729bed44-16b1-4453-ba75-12feda70a756"
            }
          ]
        },
        {
          "id": "19ede674-b75b-4b93-bc60-af27951f5a37",
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
              "id": "c834f503-f08f-43e2-8fc8-6ab4600e568f"
            }
          ]
        },
        {
          "id": "03fad2e7-71df-4645-9358-8112de697c64",
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
              "id": "8488fffb-41d2-4ef9-bf6d-cee14c7d73bf"
            }
          ]
        },
        {
          "id": "3c144f99-87a7-41f9-9df8-def7c58f607b",
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
              "id": "cb3a567c-229e-4051-8626-f899213c0460"
            }
          ]
        },
        {
          "id": "14991028-0571-43bb-929a-adb80a9e72cc",
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
              "id": "add40641-613e-418c-887c-a0105c4efc4a"
            }
          ]
        },
        {
          "id": "c737ae7b-3a09-4737-8276-190b3f6d2c31",
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
              "id": "988f56e3-5b39-42bb-b089-e1dac4477e1c"
            }
          ]
        }
      ]
    }
  ]
}