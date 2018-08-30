{
  "info": {
    "name": "BMC Software API Post an Event",
    "_postman_id": "c63808e2-0c5c-43e0-b177-7a81748cc154",
    "description": "This end point allows you to post events to the stream. You can tag them, set priority and event aggregate them with other events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "9e3957b5-d98a-4bd0-b902-9091cddc5ada",
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
              "id": "aaedbae2-6303-44bd-9fb9-23359432c08b"
            }
          ]
        },
        {
          "id": "59c04d9b-4a2d-4c2c-b519-222478ed8aad",
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
              "id": "2deae733-6529-4582-b331-20b460a16edf"
            }
          ]
        },
        {
          "id": "57410234-096b-42ab-a1f2-8258a5ed2fc8",
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
              "id": "aa89558b-e919-4c4e-9d91-13921a8e8342"
            }
          ]
        },
        {
          "id": "384b6dcc-f0cc-404c-aee9-cbc778107913",
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
              "id": "5cbadb54-6e58-40e6-af47-30636cf37ed1"
            }
          ]
        },
        {
          "id": "e879ee4b-492d-42cc-a676-cf975e804d87",
          "name": "get-all-source-information",
          "request": {
            "url": "http://example.com/api/v1/account/sources/:lastModified?",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all source (host + data stream) information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e5d3c62-8b60-4c27-81f4-c70a13e57c5b"
            }
          ]
        },
        {
          "id": "50ed14e8-f4ad-45f1-9a85-10ab7efe2f52",
          "name": "set-source-metadata",
          "request": {
            "url": "http://example.com/api/v1/account/sources",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Sets one or more source metadata"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fd2b463-bfb3-4f41-ad37-54e68a499f52"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "bb7749f6-5de2-4ab8-9892-a52c4265b40b",
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
              "id": "9bd82325-2e90-4bc5-b38d-3b84b7aabeeb"
            }
          ]
        },
        {
          "id": "de7ae5f0-c56a-4fdd-850a-946e327186e6",
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
              "id": "66faa2da-6d57-4e45-872f-c36c08104272"
            }
          ]
        },
        {
          "id": "8226d469-94e9-4fef-982f-6c14d1f65221",
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
              "id": "0ab3ce19-8cd1-44c8-9822-83ae9e223e77"
            }
          ]
        },
        {
          "id": "00ab70ee-b23d-4f15-b2ba-24e6a7fc1d6c",
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
              "id": "8041cbff-cd66-4fa4-9bb6-88e343959ed9"
            }
          ]
        },
        {
          "id": "c4e49086-013c-4a0b-9ad6-6a807f98de0a",
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
              "id": "04cf68d4-ea0d-4e6c-b70f-28e353cf80ea"
            }
          ]
        },
        {
          "id": "e59a4565-0420-411b-ad2c-6d6246ecb4f8",
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
              "id": "8fdd05fd-cefc-4daf-893e-c21fec38e922"
            }
          ]
        },
        {
          "id": "f7b56700-49b3-496c-9981-ed95d8b4ea35",
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
              "id": "4d55ae9b-0f30-473d-971a-3e2f14732198"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "5a8896e6-858d-4fa0-a23d-b398c02d8675",
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
              "id": "c4c73a59-b37b-4a7b-b993-18075acb483e"
            }
          ]
        },
        {
          "id": "761f775d-6210-463d-bdef-add66f3ca977",
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
              "id": "164327d5-7afe-4a38-a3c4-19b5c0b3555c"
            }
          ]
        },
        {
          "id": "87e91d3d-078e-4376-9ae7-c46cb6413fc2",
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
              "id": "227280eb-f4f0-44f0-b8b4-08e9220dacc2"
            }
          ]
        },
        {
          "id": "cacc4a16-aa9a-4e1e-90a1-91f992c5bda9",
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
              "id": "cba03107-1243-4b6a-b521-5361deb8e055"
            }
          ]
        },
        {
          "id": "d8f684a8-b104-4532-8e38-0f88fc85fc17",
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
              "id": "38e79af9-04d9-4741-b944-b880e966aac0"
            }
          ]
        },
        {
          "id": "6d2131e9-9bbd-40d7-b53d-8a8355b098cf",
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
              "id": "e17ce6a2-0d88-407b-a064-249e385b54fb"
            }
          ]
        },
        {
          "id": "5b2fde21-c909-4cde-98d6-a0fbc6918899",
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
              "id": "f35c29a0-16bb-453f-956b-5f5747ca8cf8"
            }
          ]
        },
        {
          "id": "a923e723-d318-4834-b143-3852e134c83f",
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
              "id": "6e4e2234-9759-4dff-8cb7-769fedc25672"
            }
          ]
        },
        {
          "id": "0b7de726-0572-41b7-af37-75bc387bf44e",
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
              "id": "01eff933-49ab-4bc3-bbf2-c135a4a03c52"
            }
          ]
        },
        {
          "id": "bc959932-3875-44c7-8202-5438e5fca85e",
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
              "id": "e4dfaabb-3b8f-410a-9bdf-0a70f5663f91"
            }
          ]
        },
        {
          "id": "14450eff-14de-49ff-bae3-c985a5bf7245",
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
              "id": "0d6dc95d-f67b-4b21-8bec-6da5a2e51b32"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "0fced463-ea1a-4494-86c8-3fd460bd2340",
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
              "id": "de4c9f66-ba0d-43fd-8765-373e8ce1a921"
            }
          ]
        },
        {
          "id": "1ae4d993-2e93-4d1c-8219-2b31857062ee",
          "name": "update-metrics-batch",
          "request": {
            "url": "http://example.com/api/v1/batch/metrics",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "type\nType of metric, could be a device metric, a plugin metric or any arbitrary type",
                  "value": "type\nType of metric, could be a device metric, a plugin metric or any arbitrary type",
                  "disabled": false,
                  "description": "descriptionDescription of the metric"
                }
              ]
            },
            "description": "Updates a batch of metrics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "192ca0e7-2bc5-4b03-90e2-61779e869d06"
            }
          ]
        },
        {
          "id": "08689443-c06c-411c-b103-581e62f809a3",
          "name": "create-metrics-batch",
          "request": {
            "url": "http://example.com/api/v1/batch/metrics",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates metrics, but in a batch"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7550eec5-9006-4b69-bdfc-daadb9be28ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "ecc1e8c5-fbbe-40c1-aea8-812dbce18457",
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
              "id": "df8672d6-c34b-42b0-b42b-85e4d2c6d3f2"
            }
          ]
        },
        {
          "id": "e4823181-782a-41d7-8857-04f7e8838abe",
          "name": "get-metrics",
          "request": {
            "url": "http://example.com/api/v1/metrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of metrics in a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f9a981c-fc72-4525-8194-dd3f51bed867"
            }
          ]
        },
        {
          "id": "fd70d2dd-ca6c-437e-ab81-c685eb1e1647",
          "name": "create-metric",
          "request": {
            "url": "http://example.com/api/v1/metrics",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name\nName of the metric, must be globally unique, recommended that you add your own namespace",
                  "value": "name\nName of the metric, must be globally unique, recommended that you add your own namespace",
                  "disabled": false,
                  "description": "typeType of metric, could be a device metric, a plugin metric or any arbitrary type"
                }
              ]
            },
            "description": "Creates a new metric"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2342b529-2fc6-44f5-bf1a-350b1bd8da2b"
            }
          ]
        },
        {
          "id": "13fd2d55-0b40-4696-840c-b883422ea186",
          "name": "remove-metric",
          "request": {
            "url": "http://example.com/api/v1/metrics/:metric",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a metric from the account.\n Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>\n flag is added."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94224b74-312f-4d04-aff5-71fd7f16853e"
            }
          ]
        },
        {
          "id": "8beb0960-e3b6-464a-93c5-eb92acdc246b",
          "name": "get-actions-for-a-dashboard",
          "request": {
            "url": "http://example.com/api/v1/metrics/dashactions/:dashboardSetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the needed configuration changes for a dashboard\n Returns an an array of objects, each has the following properties:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "090b60ce-8870-41ad-b1a2-907c454f917f"
            }
          ]
        },
        {
          "id": "fdcba8c9-1a2d-446b-a758-f5ab05e3a7af",
          "name": "perform-dashboard-actions",
          "request": {
            "url": "http://example.com/api/v1/metrics/dashactions/:dashboardSetId",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Performs necessary actions for a dashboard.\n Only enables or adds metrics at this time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5282fec-4eea-4f37-9bda-a2e2cdc549d2"
            }
          ]
        },
        {
          "id": "1a608a92-cfdd-429d-8343-1f306c5f81b9",
          "name": "update-metric",
          "request": {
            "url": "http://example.com/api/v1/metrics/:metricName",
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "type\nType of metric, could be a device metric, a plugin metric or any arbitrary type",
                  "value": "type\nType of metric, could be a device metric, a plugin metric or any arbitrary type",
                  "disabled": false,
                  "description": "descriptionDescription of the metric"
                }
              ]
            },
            "description": "Updates a metric"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea0149e0-5ae0-47f1-bd46-249cc37a70d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "29833fc9-c0a8-4416-8278-b26d34e27b52",
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
              "id": "2984c6ca-7f09-4c40-ab63-2510b158296e"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "ea77a676-636d-4986-b058-920a0008a8cd",
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
              "id": "78fc3924-8af2-478a-90d3-ebf645135dbf"
            }
          ]
        },
        {
          "id": "c2fd2d8a-4412-4ff1-af72-eefdc5058e6a",
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
              "id": "5ac88e8c-5142-4c61-8b21-da4e6481b259"
            }
          ]
        },
        {
          "id": "a1a79071-7d13-4264-b6ad-28e8b2617803",
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
              "id": "ff802f41-7f8b-4193-a095-5f824db6488a"
            }
          ]
        },
        {
          "id": "70ca9e55-3bcd-44cd-9d4b-3e5b17547ac5",
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
              "id": "878eb265-926c-49a6-ba21-3d6ac6f59e98"
            }
          ]
        },
        {
          "id": "3119bc6d-7eb9-4ac1-b2a5-92f392670148",
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
              "id": "9c6cfbd9-b99a-4373-81b9-4b9a380d85d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "21a04704-1b79-46eb-9767-ecf404f3009f",
          "name": "get-all-hostgroups",
          "request": {
            "url": "http://example.com/api/v1/hostgroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all of the Hostgroups in your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1163b158-56e0-4770-b2ce-fd67b442f7ad"
            }
          ]
        },
        {
          "id": "80dc03b7-9b7f-4b2a-8c21-536a8582a899",
          "name": "create-hostgroup",
          "request": {
            "url": "http://example.com/api/v1/hostgroups",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a Hostgroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "131c5379-b7da-442c-8d49-206346c4c10d"
            }
          ]
        },
        {
          "id": "a15b5c92-144a-44df-8d35-bff7fa5dcac7",
          "name": "search-hostgroups",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/search?name\nThe hostgroup name to search for.  Currently supported search parameters:\n\nname - search by the name of the hostgroup=name%0AThe%20hostgroup%20name%20to%20search%20for.%20%20Currently%20supported%20search%20parameters%3A%0A%0Aname%20-%20search%20by%20the%20name%20of%20the%20hostgroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Searches the hostgroups in your account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f414239-c87e-473c-ab06-e5890a21dc21"
            }
          ]
        },
        {
          "id": "09c7f0ad-947a-4b66-91e0-b30cbed2d4c3",
          "name": "get-hostgroup-by-id",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/:hostgroupId?hostgroupId\nThe Id of the hostgroup you are requesting=hostgroupId%0AThe%20Id%20of%20the%20hostgroup%20you%20are%20requesting",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a single hostgroup by its id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8b99afd-2b83-4a41-8f7f-cb7a5b8322d9"
            }
          ]
        },
        {
          "id": "e6df3166-5471-449f-8028-7261b8258d77",
          "name": "update-hostgroup",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/:hostgroupId",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a Hostgroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63771e29-1f6a-490e-a3e4-c189a5f61c5b"
            }
          ]
        },
        {
          "id": "f268af75-7c7b-4c3e-b478-9d4fb36d3635",
          "name": "delete-hostgroup",
          "request": {
            "url": "http://example.com/api/v1/hostgroups/:hostgroupId?hostgroupId\nThe hostgroup to delete\nforceRemove\nRemove the hostgroup, even if it&#39;s being used by a dashboard or alarm=hostgroupId%0AThe%20hostgroup%20to%20delete%0AforceRemove%0ARemove%20the%20hostgroup%2C%20even%20if%20it%26%2339%3Bs%20being%20used%20by%20a%20dashboard%20or%20alarm",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an hostgroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92ac5218-e630-428b-9e78-bc7a4acc6b88"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "9bd060a8-6efd-45a6-97c4-b609f90e76f2",
          "name": "registration",
          "request": {
            "url": "http://example.com/api/v1/meter/:meterName/registration",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "meterVersion",
                  "value": "meterVersion",
                  "disabled": false,
                  "description": "What version of the Meter is running, ex"
                }
              ]
            },
            "description": "Register a Meter with TrueSight Pulse"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc9feeff-f96c-49cf-a1d1-bc71e01a315f"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "76867029-692a-4780-8f2a-df21b84597f0",
          "name": "add-measures",
          "request": {
            "url": "http://example.com/api/v1/measurements",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "source",
                  "value": "source",
                  "disabled": false,
                  "description": "The source of the metric"
                }
              ]
            },
            "description": "Adds measurement readings to the data store."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5b03d5a-ecf9-4dc7-a917-63311b2c4ec6"
            }
          ]
        },
        {
          "id": "a6282d26-3b43-4894-969d-0f4de56fb142",
          "name": "get-measures",
          "request": {
            "url": "http://example.com/api/v1/measurements/:metric",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves measurement readings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27c93a41-9e1c-44eb-8cda-4575b408e2ea"
            }
          ]
        },
        {
          "id": "3ec1ed35-eb6b-4e1d-8bd0-94957ab8100c",
          "name": "get-measures-batch",
          "request": {
            "url": "http://example.com/api/v1/measurementsBatch",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Same as /v1/measurements/:metric except that an array of query objects are passed in the body."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad18b3a8-d3a4-452f-a14d-cd1c7eae4443"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "830c76b5-d5d1-4cf2-af1f-68d6054c64f6",
          "name": "get-all-plugins",
          "request": {
            "url": "http://example.com/api/v1/plugins",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all known plugin definitions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abbb4a16-d9f8-4cf9-9faa-cf4a5b17d5d1"
            }
          ]
        },
        {
          "id": "0ca757f1-f660-4169-acec-c9527e7fbf18",
          "name": "get-plugin-components",
          "request": {
            "url": "http://example.com/api/v1/plugins/:plugin/components",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds the components associated with an installed plugin including metrics and dashboards"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06806611-937a-4cc3-8b1f-98a407674bb8"
            }
          ]
        },
        {
          "id": "1be22b60-b9e5-4519-bf62-18936624368a",
          "name": "get-installed-plugins",
          "request": {
            "url": "http://example.com/api/v1/plugins/installed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets plugins that are installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f29bab98-1a86-446b-8749-56dac892c6ea"
            }
          ]
        },
        {
          "id": "c2087b05-03a4-47d1-9d31-305f4b5d4895",
          "name": "install-or-update-plugin",
          "request": {
            "url": "http://example.com/api/v1/plugins/installed/:plugin",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Installs a plugin"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1633cf34-35d5-402f-9cf5-bba84f065c8b"
            }
          ]
        },
        {
          "id": "103f0964-2717-4bae-bf65-a446349cb7e1",
          "name": "uninstall-plugin",
          "request": {
            "url": "http://example.com/api/v1/plugins/installed/:plugin",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Uninstalls a plugin and optionally removes related dashboard(s) and metric(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a59a91cc-2644-4008-82ea-2978d26af3e9"
            }
          ]
        },
        {
          "id": "43974220-3e37-430b-8263-ab624fa04d17",
          "name": "add-private-plugin",
          "request": {
            "url": "http://example.com/api/v1/plugins/private/:plugin/:org/:repo?plugin\nName of the plugin\norg\nGithub organization or user owning the plugin\nrepo\nGithub repository name for plugin=plugin%0AName%20of%20the%20plugin%0Aorg%0AGithub%20organization%20or%20user%20owning%20the%20plugin%0Arepo%0AGithub%20repository%20name%20for%20plugin",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or updates a private plugin.\nA plugin exists as a repository in Github.\nBy adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which\ncan then be installed and/or added to a relay.\nIf a private plugin has the same name as an existing plugin it will override the existing plugin within your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9bad091-5fce-45f5-8873-d3ea9e2d4446"
            }
          ]
        },
        {
          "id": "8a02b4df-65b8-46b6-af37-f545f1e183fb",
          "name": "remove-private-plugin",
          "request": {
            "url": "http://example.com/api/v1/plugins/private/:plugin?plugin\nName of plugin to remove=plugin%0AName%20of%20plugin%20to%20remove",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a private plugin from your account. Use this function after adding a private plugin to make your private\nplugin disappear from available plugins in your settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b237886-4c35-4369-a02d-858080370b40"
            }
          ]
        },
        {
          "id": "dd96ac8b-53c2-4510-8c36-1e9b6a14198e",
          "name": "get-plugin",
          "request": {
            "url": "http://example.com/api/v1/plugins/:plugin?plugin\nName of plugin=plugin%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single plugin definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c0a7f73-8330-444d-9788-3ba2b7e58818"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "bac94c03-ed41-49f6-abf1-0caa8a577619",
          "name": "set-relay-heartbeat",
          "request": {
            "url": "http://example.com/api/v1/relays/heartbeat",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the &#39;lastHeardFrom&#39; field of the relay configuration\nReturns the current system time in UNIX epoch of server."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c56daa92-1737-4565-a1da-6957eca786f4"
            }
          ]
        },
        {
          "id": "57dc6ca6-d5df-4298-9154-c36331a6344d",
          "name": "get-all-relay-configurations",
          "request": {
            "url": "http://example.com/api/v1/relays",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the configurations for all visible relays"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "212367a8-546c-4178-bf74-0d953f2cf79d"
            }
          ]
        },
        {
          "id": "7dec1ebc-fca1-4bd6-b476-7a776aaabf18",
          "name": "get-relay-configuration",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/config",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves config for a relay host if changed\nIf no timestamp specified, configuration data is always returned\nIf config has not changed the string &#39;not-modified&#39; is returned"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dc79435-a197-419c-b4c3-c549b26e16ab"
            }
          ]
        },
        {
          "id": "354320e6-02b1-4a02-b22a-e77eb0331556",
          "name": "set-relay-configuration",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/config",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Stores configuration for a relay.\n The relay will gather the configuration on the next poll and reconfigure itself as needed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de8dd252-fbb3-4676-a2e3-9abd518a74db"
            }
          ]
        },
        {
          "id": "7b1b1114-9827-42a6-8161-b68b424d26cf",
          "name": "toggle-relay",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/toggle?relay\nName of relay to toggle=relay%0AName%20of%20relay%20to%20toggle",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "disabled",
                  "value": "disabled",
                  "disabled": false,
                  "description": "true or false"
                }
              ]
            },
            "description": "Set a relay to be disabled or enabled"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec0145cf-d57d-46a1-9cff-721daff4caf3"
            }
          ]
        },
        {
          "id": "537f5646-fd69-490f-874b-cb8589bf1689",
          "name": "toggle-relay-plugin",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/togglePlugin",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "plugin",
                  "value": "plugin",
                  "disabled": false,
                  "description": "Name of plugin"
                }
              ]
            },
            "description": "Sets a relay plugin to be disabled or enabled"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08b5498a-c5c0-47a1-b267-6d7d5381e820"
            }
          ]
        },
        {
          "id": "908b2281-3edd-451f-92ea-b039cc18dd74",
          "name": "add-relay-output",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/output",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds output messages to the relay.\nUsed by the relay to communicate output from execution and commands"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68c63235-aa4c-4173-b52a-cb384083e122"
            }
          ]
        },
        {
          "id": "2a87cacb-0823-4480-95d1-6539c7b188d3",
          "name": "clear-relay-output",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/output",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Wipes the logged output from the relay up to present."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59c4521b-f87e-48c4-834e-9fa9f77e5c85"
            }
          ]
        },
        {
          "id": "b7446e41-34b7-40c8-b641-9fed7f0303e4",
          "name": "get-relay-output",
          "request": {
            "url": "http://example.com/api/v1/relays/:relay/output/:since",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Queries for relay output messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19f24d05-1be5-4a5f-b528-576ebf6cfec7"
            }
          ]
        }
      ]
    },
    {
      "name": "Sources",
      "item": [
        {
          "id": "d96727d3-d5cc-438b-910a-13d842f1af3a",
          "name": "remove-old-sources-by-name",
          "request": {
            "url": "http://example.com/api/v1/sources/byName",
            "method": "DELETE",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "names",
                  "value": "names",
                  "disabled": false,
                  "description": "An array of source names to delete"
                }
              ]
            },
            "description": "Remove Old Sources from your account by using a list of names"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0927b82b-b765-40b7-8f06-cf7a8863982f"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "b3f3b1f9-11da-4f92-bb09-f917c50d7ee2",
          "name": "get-list-of-active-metrics",
          "request": {
            "url": "http://example.com/api/metrics?[[POSIX_timestamp, numeric_value], ...]=%5B%5BPOSIX_timestamp%2C%20numeric_value%5D%2C%20...%5D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of actively reporting metrics from a given time until now. This endpoint is not available in the Python and Ruby libraries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eed71201-3f22-4733-a734-6d382ce598a2"
            }
          ]
        },
        {
          "id": "e424a5e9-4ed2-4f4a-b9af-465f0a31557f",
          "name": "post-an-event",
          "request": {
            "url": "http://example.com/api/api/v1/events",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This end point allows you to post events to the stream. You can tag them, set priority and event aggregate them with other events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4a380f3-fdc6-4aaa-9473-ff6b48e349e7"
            }
          ]
        }
      ]
    }
  ]
}