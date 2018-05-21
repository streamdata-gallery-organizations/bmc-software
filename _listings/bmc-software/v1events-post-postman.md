{
  "info": {
    "name": "BMC Software API Create event",
    "_postman_id": "07278e5f-bdfc-4bd2-ae23-9ae16097aa1d",
    "description": "Creates an event. Every event occurrence is persisted to the database as a RawEvent. Based on the EventFingerprint, a new Event will be created or an existing one will be de-duplicated.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "8b761215-ddb4-4ae9-a3ce-36d4d6b3cc8e",
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
              "id": "6e023405-37ff-47b1-8f49-45aa0cb341ab"
            }
          ]
        },
        {
          "id": "03175214-d922-4d7c-8a3e-9ce9ed368e33",
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
              "id": "2fd0b790-4928-4c6e-935a-cc122bc89354"
            }
          ]
        },
        {
          "id": "2af44206-4871-4f78-833b-e19f8e282bc1",
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
              "id": "84c3cce9-f508-48f5-9f29-71c0d6ddca54"
            }
          ]
        },
        {
          "id": "245a62b3-1771-470e-8a32-4520bec5b639",
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
              "id": "6be10ca9-c3af-4b42-a73b-7a631ab932f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "6c45159c-55e6-46da-817b-f5e2e2bb0c42",
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
              "id": "ed8370d8-10f5-44ad-9aa7-cbe226e4c8e9"
            }
          ]
        },
        {
          "id": "d59ca5a5-aff6-454c-8b55-fac9e399e986",
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
              "id": "7624273d-3078-4695-b315-4f796d5fd426"
            }
          ]
        },
        {
          "id": "fb21f2c7-50d8-4da7-ad90-da54ed05e392",
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
              "id": "2a215101-c278-4350-bbde-3ed83f44745c"
            }
          ]
        },
        {
          "id": "7442a558-cf2a-497e-8237-2e6f29ce6748",
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
              "id": "218542ef-c085-4b4e-8acb-1cdc487d3e66"
            }
          ]
        },
        {
          "id": "2f4d43b3-3ed0-4031-af5f-f2168d697785",
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
              "id": "d39a6b07-0d3b-47f8-af38-30a424cdd58a"
            }
          ]
        },
        {
          "id": "4b991a1e-bb25-41ba-832c-1cf2c40c7684",
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
              "id": "196c1184-82e8-4445-96dd-b96305f6f91f"
            }
          ]
        },
        {
          "id": "50f73bfa-d9db-430c-987f-10d6e1388406",
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
              "id": "490279f0-4a87-4ab7-9626-cb083c8880ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "14f43bad-e70e-47f9-aa1e-d1c2d05cfd01",
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
              "id": "0c5bc8b4-7eaa-4b34-8678-2f6f449d2240"
            }
          ]
        },
        {
          "id": "ad9f2056-d593-47ad-b509-004a84a11095",
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
              "id": "ea3470ce-15ba-42d7-a180-83afa84b2d13"
            }
          ]
        },
        {
          "id": "4b2e16c4-99ec-4fc2-aee5-c187e4451b85",
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
              "id": "4e370f8c-9cdc-4a79-b420-fd94ccd2807a"
            }
          ]
        },
        {
          "id": "c8e8b927-2077-4686-88be-bce7dad27a37",
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
              "id": "a64cbfc0-bfc9-48af-a5ed-b3017384e34d"
            }
          ]
        },
        {
          "id": "7096e6ef-1275-41c3-a23c-377a3fb0f27b",
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
              "id": "68f046d7-1d02-4163-90e1-81a43134cc3d"
            }
          ]
        },
        {
          "id": "e1859a24-54bb-4fac-9c43-de7f63f5d588",
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
              "id": "0767759b-0cd9-4ec9-ba9f-2bb7cd64993d"
            }
          ]
        },
        {
          "id": "eb5636f4-a211-4925-88d9-64063045a3ea",
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
              "id": "e697848e-2e62-44a0-ba72-5dad7d64fe28"
            }
          ]
        },
        {
          "id": "3a0bfc9e-3f1c-406a-a93b-96394774b385",
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
              "id": "033718c1-e6be-4eba-bf10-7c227c268e49"
            }
          ]
        },
        {
          "id": "4601f3f2-2e66-461c-b589-745cab5e5ec8",
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
              "id": "45bd13c4-4146-4571-a8e9-660f56baa9c1"
            }
          ]
        },
        {
          "id": "ea6fb14b-88bc-41d4-829a-ca654f334f98",
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
              "id": "2946399a-b5c9-49c9-9046-b347e4f0765e"
            }
          ]
        },
        {
          "id": "9fcae142-74d0-4756-8b3c-9e7492f4027f",
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
              "id": "2d1bb02d-135c-40cb-b39b-84df2adc0ef9"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "0fa658d8-99e1-45eb-abfa-2620d35f6992",
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
              "id": "674e5dfe-94a2-41d3-b6b5-4f6443db8a9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "a27b36b5-ac0e-4862-b5be-bd27fb323838",
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
              "id": "9736d3a4-debf-4b7f-9156-22d1e53c1581"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "c0892229-da3f-4c64-95c7-10be4b40cf97",
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
              "id": "fd294072-92b6-4b68-b729-90dfb27c0ec3"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "4f5f3cdc-5d82-4060-ad2b-4e7fff4971a9",
          "name": "create-event",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an event. Every event occurrence is persisted to the database as a RawEvent. Based on the EventFingerprint, a new Event will be created or an existing one will be de-duplicated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fdefe4c-0051-42d4-be2c-f420488127cc"
            }
          ]
        }
      ]
    }
  ]
}