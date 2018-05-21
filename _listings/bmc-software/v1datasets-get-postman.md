{
  "info": {
    "name": "BMC Software API List dataset",
    "_postman_id": "6eac54a0-4c09-4a9e-86c8-a79e122f46de",
    "description": "*",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "1858e01e-9f83-401d-8342-0991d7e941ea",
          "name": "information-about-the-authorized-account",
          "request": {
            "url": "http://example.com/api/account",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the authorized account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "420e1fb8-de43-4acd-9ed8-f2bb02e15fc8"
            }
          ]
        },
        {
          "id": "68a55124-b841-4a87-8c41-3601f544d0a7",
          "name": "get-aws-integration-status",
          "request": {
            "url": "http://example.com/api/v1/account/aws/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets AWS status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "655261c9-d9fc-4233-931a-608d403f200e"
            }
          ]
        },
        {
          "id": "e2ee6276-130e-4ccd-939d-42af090c9da6",
          "name": "delete-account-mobile-device",
          "request": {
            "url": "http://example.com/api/v1/account/mobile-devices/:accountDeviceId?accountDeviceId\nThe account device ID to delete=accountDeviceId%0AThe%20account%20device%20ID%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device from an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73e8ab71-ee6d-4a57-a9a7-9e458848c34c"
            }
          ]
        },
        {
          "id": "7d85bd6d-ae09-4dba-86a7-e4df66b23330",
          "name": "get-all-account-mobile-devices",
          "request": {
            "url": "http://example.com/api/v1/account/mobile-devices",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all of the devices for an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efcf3a80-55e9-4aa6-a5f4-bb914f1fb012"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "69f9a24e-86b2-4c0f-a982-2549999dbd6f",
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
              "id": "bb1595b9-b80d-43a9-a42e-863f05f84eb4"
            }
          ]
        },
        {
          "id": "a063c8fb-5229-42d0-b325-f384c64fcd3d",
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
              "id": "7a840b63-0732-4e2d-af1c-c2264ec5f27e"
            }
          ]
        },
        {
          "id": "2784846b-e920-4896-a825-4556105bdfb3",
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
              "id": "99d50b02-1100-48b6-a5e7-e0d792fbe4df"
            }
          ]
        },
        {
          "id": "f7153fbd-48ac-47cd-8918-d9127b61aa65",
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
              "id": "c8a4e392-6506-4bdb-8e08-9b87736b9b2b"
            }
          ]
        },
        {
          "id": "39bdcbd4-1738-45dc-8415-7288211027fc",
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
              "id": "fa4ab345-29d4-4c24-93e4-bad18ea139e3"
            }
          ]
        },
        {
          "id": "7b81adc5-bf78-48d1-837f-99933c333ec2",
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
              "id": "db26e985-46f1-4af9-b8f6-049a43cd14ed"
            }
          ]
        },
        {
          "id": "58c0fe6f-d127-442c-8362-536d40272ba8",
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
              "id": "8c991133-4fa3-4138-bdfb-a515eec7608b"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "d45fffce-7a4e-48cb-8d55-661dce0b7fd1",
          "name": "get-all-alarms",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Alarms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1def19e7-edc0-483b-b18e-d7874232a0f1"
            }
          ]
        },
        {
          "id": "5a843594-f96f-46aa-ac3f-8e4be39abe39",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarms",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cdb44df-1e94-4760-b537-af7d05c85d75"
            }
          ]
        },
        {
          "id": "f447a0cf-e14e-4b65-9e7d-bf152a8f05f4",
          "name": "get-alarm-by-id",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId=alarmId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02115e2e-e182-46b4-a163-b3136512d567"
            }
          ]
        },
        {
          "id": "f7ff201a-2ad3-46e0-8bcc-7e46ce491415",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false,
                  "description": "The name of the alarm"
                }
              ]
            },
            "description": "Update an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ca22376-6dd7-4f1b-9a7a-eea4b5e891b8"
            }
          ]
        },
        {
          "id": "1237df39-b91d-4aab-a086-76992f9b91b3",
          "name": "delete-alarm",
          "request": {
            "url": "http://example.com/api/v1/alarm/:alarmId?alarmId\nThe alarm to delete=alarmId%0AThe%20alarm%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5403d25-40e0-4622-a423-145ee22c71f9"
            }
          ]
        },
        {
          "id": "f0205cfb-ae91-4781-81ab-0968423fbdd7",
          "name": "get-alarms-by-name",
          "request": {
            "url": "http://example.com/api/v1/alarms/search?alarmName=alarmName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves alarms by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18914e2-f15b-4347-bc87-3f94ee64e895"
            }
          ]
        },
        {
          "id": "6400dc40-60d9-494a-bc96-8838ef8e8316",
          "name": "get-all-alarms1",
          "request": {
            "url": "http://example.com/api/v2/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Alarms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34e05478-ac35-44bf-8646-2f8c3e472dd1"
            }
          ]
        },
        {
          "id": "d38ec0a7-7b0b-44a0-a6ca-b9723929d887",
          "name": "create-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1d40f46-00c3-4510-9480-1bc332a13282"
            }
          ]
        },
        {
          "id": "bcde1838-68ed-4d8f-8f82-faf8f1e8f4f4",
          "name": "get-alarm-by-id1",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId=alarmId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b2cedb0-c938-4cca-86c8-3b14c1156821"
            }
          ]
        },
        {
          "id": "5df9dcfe-1e0b-4435-95ee-3514c0530fb2",
          "name": "update-alarm",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId integer\nThe alarm to update=alarmId%20integer%0AThe%20alarm%20to%20update",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8d78ad8-ceee-49fb-bbb0-e50089a44e02"
            }
          ]
        },
        {
          "id": "2491fff5-d6af-4a05-af9c-ba049e24168a",
          "name": "delete-alarm1",
          "request": {
            "url": "http://example.com/api/v2/alarms/:alarmId?alarmId\nThe alarm to delete=alarmId%0AThe%20alarm%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an alarm"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6410063-31a9-4481-93a3-da02452d5654"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "48349ee5-8369-4457-a3a7-af8b8245cab3",
          "name": "perform-batch",
          "request": {
            "url": "http://example.com/api/v1/batch",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows making an arbitrary set of API calls.    All calls are made in parallel.\nThe query string parameter <em>?series</em> can be used to override this behavior and call the API in series stopping at the first error."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69514a7a-33df-4ff8-875a-23121daeca83"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "3d7556aa-df16-4d54-a69a-c1a02807a084",
          "name": "delete-mobile-device",
          "request": {
            "url": "http://example.com/api/v1/mobile-devices/:userDeviceId?userDeviceId\nThe user device ID to delete=userDeviceId%0AThe%20user%20device%20ID%20to%20delete",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device from a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3465c253-a24e-4b07-bfca-fbbd48a8399f"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "16d39cc4-6a15-47d9-beec-d33edc0f3285",
          "name": "list-dataset",
          "request": {
            "url": "http://example.com/api/v1/datasets/*",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "*"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f81a855f-ab15-4222-899c-6c58791f94f2"
            }
          ]
        }
      ]
    }
  ]
}