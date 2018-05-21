{
  "info": {
    "name": "BMC Software API Get raw events",
    "_postman_id": "540a1095-bdc2-496d-9021-bea9285140af",
    "description": "Returns all of the event occurrences (raw events) for the specified event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "91e8e76e-9a0b-41b5-8611-9d5a7b0b10e9",
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
              "id": "d894c006-aeb1-42fa-8119-523c3e494f1c"
            }
          ]
        },
        {
          "id": "990a0bd5-70c8-487d-9b73-f2165235f990",
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
              "id": "d09e5b77-8477-44e8-afbb-e8096415e4ae"
            }
          ]
        },
        {
          "id": "fbe2c77f-36bb-4dd1-b7c4-d4ff6068ea9d",
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
              "id": "dcadd736-ca12-4787-816a-5cf686197ce3"
            }
          ]
        },
        {
          "id": "09503733-bef7-4464-99c8-02d8aab9261d",
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
              "id": "2f6ca4bf-9f03-4be6-b768-b89dce3841e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "3c4fccaa-0d1d-4256-844a-2c22a7ed69ca",
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
              "id": "3dbf2261-f196-41f7-b622-099014424122"
            }
          ]
        },
        {
          "id": "b4a91256-8bf7-43bd-9869-37a44249581d",
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
              "id": "8a37fe97-475e-4fbe-a967-bd1656299ecd"
            }
          ]
        },
        {
          "id": "8bdfc63d-5c8b-4fab-b1eb-69f0424e3bc3",
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
              "id": "71a7b27b-5b28-4e73-9c5e-8bf90d475110"
            }
          ]
        },
        {
          "id": "33925499-01e1-40aa-9441-7307ddb7c2a6",
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
              "id": "b1a33117-3d7c-4ac3-be5f-c04985411b21"
            }
          ]
        },
        {
          "id": "a881c631-263f-41b0-8ca1-3ace6d350d12",
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
              "id": "c272832e-b461-4b05-8c28-887c898c5d3b"
            }
          ]
        },
        {
          "id": "a05a7496-c85b-40bc-8108-dea5039a43ae",
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
              "id": "57c6a307-7bf6-4359-829a-eec2551be3ae"
            }
          ]
        },
        {
          "id": "e40842a5-af47-4f9b-8256-14578bfb5da2",
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
              "id": "b9c4b855-d46c-45c8-b6f5-01044aa067dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "897ec9f4-877a-4f08-90c5-aa2f8c5f988d",
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
              "id": "6179f5b7-7b0b-4763-939e-538a4c86b189"
            }
          ]
        },
        {
          "id": "8a8fb34f-c09d-4c0e-86d9-19313aaeb120",
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
              "id": "309b8de6-0aaf-4591-b45c-480d21d46729"
            }
          ]
        },
        {
          "id": "6e792754-2a05-413d-b6b2-b818b789d9a0",
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
              "id": "d59bc77a-1e8a-45f0-ae2d-c38dacdae777"
            }
          ]
        },
        {
          "id": "dce5a45a-b90a-4d37-aa9e-a2c158cdac46",
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
              "id": "15d98b23-f9f8-4b62-8b1e-1ad550808ee9"
            }
          ]
        },
        {
          "id": "c933b978-d07d-44c6-bc38-07531ac40441",
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
              "id": "5df34f02-04a0-4d70-ad3b-8d8d6d9b8bf7"
            }
          ]
        },
        {
          "id": "c1072801-b950-435e-a873-bd90aa06b9b6",
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
              "id": "620cae36-94fa-4312-8a98-b1d39c32ab57"
            }
          ]
        },
        {
          "id": "b31627ac-1147-451d-b297-80e178612e39",
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
              "id": "4533b846-2e24-44a9-8844-8948665b07dd"
            }
          ]
        },
        {
          "id": "ed8d262d-c415-4309-a4f8-8b9da354cabc",
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
              "id": "7e5e7684-b95e-4b24-9755-178bc0803b11"
            }
          ]
        },
        {
          "id": "b61327dc-2ea0-4fa3-8c8e-73158e919610",
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
              "id": "324d7bdf-a464-4e9f-a85e-063b07cea00b"
            }
          ]
        },
        {
          "id": "3610b22c-4e00-4c28-8392-939858ca0bb6",
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
              "id": "8e176154-0e1d-4eaf-803f-a427cc483a1e"
            }
          ]
        },
        {
          "id": "a0523cb8-b75b-4782-a528-6e8a615d2045",
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
              "id": "75307597-ff3a-4d50-9518-051edcea67ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "dba74774-b530-43d4-9bff-fe089a450ab5",
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
              "id": "a07fba5f-c6c7-4d22-9cf9-ce426b2cd42b"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "96327e81-f7a2-440f-9ee6-76907523f51b",
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
              "id": "4e453ff5-2970-487b-888a-df29c2d96b06"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "050e1b30-bb78-4e24-85f5-5ba69e623126",
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
              "id": "7ebe6c0c-cbd1-4229-a9df-3a2c0a8b3320"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "1985e501-adff-46df-8ce2-7c1136b9e49d",
          "name": "list-events",
          "request": {
            "url": "http://example.com/api/v1/events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches for events in the specified organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cb53f17-7690-4aac-8e8d-b1475e8c025a"
            }
          ]
        },
        {
          "id": "ba7e2ba3-eeaa-493e-98b7-d4553eb8f39c",
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
              "id": "b8fe4596-4e55-4a46-80b8-6a37a5051139"
            }
          ]
        },
        {
          "id": "02bbb1f1-e763-48f5-a230-75a06eca3b9e",
          "name": "list-raw-events",
          "request": {
            "url": "http://example.com/api/v1/events/raw",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Queries all event occurrences (raw events) for the specified organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1111a4d-a440-4507-afa7-455d2af72860"
            }
          ]
        },
        {
          "id": "7f26b03f-cfd7-4209-85c9-099be00e1632",
          "name": "get-event",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the event with the specified event id from the database."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57cc26a3-8334-4a74-b7fd-7235bde872d3"
            }
          ]
        },
        {
          "id": "f4aac939-d9c2-4af5-9c68-766e1f6b937b",
          "name": "get-raw-events",
          "request": {
            "url": "http://example.com/api/v1/events/:event_id/raw",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the event occurrences (raw events) for the specified event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61f725a9-f1ae-49dc-ba35-536900952f98"
            }
          ]
        }
      ]
    }
  ]
}