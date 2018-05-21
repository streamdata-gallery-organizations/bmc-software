{
  "info": {
    "name": "BMC Software API Add relay output",
    "_postman_id": "a439fa3b-e024-4ee1-a0c6-0f728c398b83",
    "description": "Adds output messages to the relay.\nUsed by the relay to communicate output from execution and commands",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "560d353f-96d5-45b1-8c47-0beb08709de8",
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
              "id": "8c5785aa-594e-4879-b717-17a09b49b4ea"
            }
          ]
        },
        {
          "id": "fc6866f9-9098-47e6-bc9c-4fe5edacc40e",
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
              "id": "20e0b8c3-a38d-4463-9b92-bb31eb0d5c1a"
            }
          ]
        },
        {
          "id": "6b25e6d9-6af5-4ad1-b883-a92c4900aacd",
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
              "id": "a4bd65f1-aa4b-4d9e-a162-a8306e56eaef"
            }
          ]
        },
        {
          "id": "88135414-bdce-4acc-af1d-9db0d44584f4",
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
              "id": "009ee918-b4cd-4b19-a516-c46ab6459f0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "579d42c0-2c48-4909-99af-1c0d79bc0f47",
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
              "id": "39df44f4-1b40-4d41-bc5c-4cc53f06b716"
            }
          ]
        },
        {
          "id": "ea2b2511-7267-428f-b8f7-56392430d2e4",
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
              "id": "3206efe3-ae80-457e-9bcf-a3d2e701f17d"
            }
          ]
        },
        {
          "id": "aebd5a59-cc50-4809-a699-c4d96fc193be",
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
              "id": "a16bf297-da72-4b7d-b767-d9fa0f2da1ff"
            }
          ]
        },
        {
          "id": "fa779960-a785-48b8-bd19-bae75a076fab",
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
              "id": "faa02d8d-3701-4856-b021-13fb451ffa35"
            }
          ]
        },
        {
          "id": "ac6fc3f9-1025-409f-b27f-6dc5f1db5b60",
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
              "id": "9de33ba2-4437-4734-b061-90c519c2b443"
            }
          ]
        },
        {
          "id": "930e8a62-d3d1-4b1a-9168-1d5031a91643",
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
              "id": "3c5e6bc1-83c5-4091-934f-af01ead50163"
            }
          ]
        },
        {
          "id": "056843ef-517e-49a3-898a-f27f395b64d4",
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
              "id": "fe98046b-dbf5-4f2a-9734-e161d5de7cca"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "50e7b23b-895a-4212-bd54-b06eabae9812",
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
              "id": "ab0a5dd4-d8c0-4e9e-8ff3-ef05f1eb4bb4"
            }
          ]
        },
        {
          "id": "d24f2d40-fde4-407d-bbc9-0ca7c922feea",
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
              "id": "4779d9e0-1e11-4fcb-ad48-0aa12898251f"
            }
          ]
        },
        {
          "id": "e29d7904-d9c3-4a23-a311-5abfc3bc0ceb",
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
              "id": "c52d928c-5a8f-4397-90a1-faac44ea44cb"
            }
          ]
        },
        {
          "id": "b50c86a3-9378-4ca4-b3d0-1d1c38816800",
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
              "id": "f9f58804-ab12-4e43-9fea-63588be79c98"
            }
          ]
        },
        {
          "id": "86f7dc4a-c10f-4e9c-987e-fe4e47dad7cf",
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
              "id": "059e549d-7c41-44f3-aeca-d97ed5a2110f"
            }
          ]
        },
        {
          "id": "aa06ebb1-ad49-408f-813c-41b6a5cb8f7b",
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
              "id": "3e33e7c3-7a04-4313-ae54-24ee031e076a"
            }
          ]
        },
        {
          "id": "013fce3c-00e3-4597-8698-bda11d74a7d5",
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
              "id": "92edf65e-6a58-4755-92e1-013ee8f2f08a"
            }
          ]
        },
        {
          "id": "7532b5f4-9093-4739-a2db-74c4c3b56647",
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
              "id": "7e7a2318-819f-4a45-906e-8d61108c174e"
            }
          ]
        },
        {
          "id": "2bd5e0af-9d2d-4bbe-85dc-2ae659713eef",
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
              "id": "cc96c5a2-b4e0-4519-84ef-ffc01f76aa26"
            }
          ]
        },
        {
          "id": "3dfa11d2-416d-4287-8f13-f539361acc68",
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
              "id": "c22af033-b255-44c4-9517-8cb87675c137"
            }
          ]
        },
        {
          "id": "25ab1702-5107-4eb4-afc0-914d0ccd0890",
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
              "id": "c1d9c061-d035-4323-a915-c926cb6cc8db"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "aab69479-dba7-48b9-a562-fb9d68035de0",
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
              "id": "51b19cfb-2878-45be-b38c-09d06f0a8cb1"
            }
          ]
        },
        {
          "id": "274db6d9-d0f5-491a-9e10-898fdd9b0dee",
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
              "id": "c11bcfb7-ea55-486b-b5ac-d205f6690c91"
            }
          ]
        },
        {
          "id": "16b742c0-c59a-4aec-8917-4099a5ace570",
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
              "id": "4e31c136-f0e0-48e9-a075-4b7563ff9376"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "f7e08aca-df7a-4402-a5b5-e78fe3c52351",
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
              "id": "01b0b8fc-2cfd-4605-b7d1-9a0417e7a1db"
            }
          ]
        },
        {
          "id": "cc0036a8-ba50-4b50-bba3-8953189da650",
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
              "id": "871a140b-b48f-43ab-b57b-04092f78c057"
            }
          ]
        },
        {
          "id": "1bd3ec90-33eb-45b7-9ecf-ae18eaa099bc",
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
              "id": "d3b503c1-0711-410e-b0e0-a273e6a4c588"
            }
          ]
        },
        {
          "id": "b1cef535-5ad6-42b9-84e6-af06428cc2ec",
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
              "id": "04c33895-0ab1-47a8-9b1a-ede81d49ff04"
            }
          ]
        },
        {
          "id": "3e8e8fa9-d1c0-4d02-a89b-ca7eee41b080",
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
              "id": "63f13591-2aff-46bf-8159-6a92c64753c2"
            }
          ]
        },
        {
          "id": "dc6fb317-250b-4e0c-a195-86abf1b0a8fa",
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
              "id": "b9c56099-df11-48b6-a936-ae9d4a87e709"
            }
          ]
        },
        {
          "id": "7f59f7f4-3ae2-42b2-9673-18479379629d",
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
              "id": "c3b161c4-4123-424f-ac1b-712b70a6879a"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "2febe484-156c-448a-9230-ae09c6a5ee28",
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
              "id": "832de2d6-c06b-466d-8666-0d76e6e941a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "8cc03938-7f30-4324-ace8-99bce1b88991",
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
              "id": "8faf181a-b00a-4e55-ab8f-750dc4ea3898"
            }
          ]
        },
        {
          "id": "06697d73-e8e9-479c-8959-0d37335ed6a2",
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
              "id": "27d314df-45c8-44de-80d4-b615ccdc82ff"
            }
          ]
        },
        {
          "id": "59034866-59ce-417c-828e-717feb8b46ad",
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
              "id": "bd647cec-de34-448c-9124-4f8b9eeeedef"
            }
          ]
        },
        {
          "id": "7ad2bec3-9260-4ebb-8c18-0e036b58a88f",
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
              "id": "523e9fa1-cf77-47c0-8d0f-23347fc7bcc1"
            }
          ]
        },
        {
          "id": "a0d56992-6693-4770-a434-a63fd29f9ba4",
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
              "id": "20f9e329-b621-482f-bd35-511c04e0cb00"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "87461b7c-87f7-4fe6-b91e-57e4eee257ce",
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
              "id": "b47e0c4f-7944-4565-9a5a-47bdd65281c1"
            }
          ]
        },
        {
          "id": "73988f67-e816-47f1-a149-80c0f11e22b5",
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
              "id": "774a9744-aa7b-4873-8d86-b4b542dd6475"
            }
          ]
        },
        {
          "id": "6a3ea5c0-8384-416e-8b22-72af44a4bcb6",
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
              "id": "4b3010d2-df09-4139-ae08-50d7555a9fe6"
            }
          ]
        },
        {
          "id": "522893ad-7d24-4b0a-aa6d-22b65b217ad9",
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
              "id": "0c6ed669-9ea6-420a-8fec-7b6a1f72eb4d"
            }
          ]
        },
        {
          "id": "5fed5799-7e62-42c7-879b-e120a9f24165",
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
              "id": "45683950-9de4-43fb-9e21-e95d55e5a443"
            }
          ]
        },
        {
          "id": "2d8a9b8c-8c45-4fe6-9d27-0cf74ecc4182",
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
              "id": "77cdfddf-d076-4c3f-b38b-f836ed5c2b4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "f65f2080-a124-4b23-a8fa-28d952deae74",
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
              "id": "2bd4f42f-6ba6-4113-80e0-3e26ff19f6e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "cf6439f0-9207-471a-a8df-fb98bea8d063",
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
              "id": "4ab51315-eab8-431e-a856-e8de58d43cda"
            }
          ]
        },
        {
          "id": "84cc6b68-9bf5-4a5a-aba8-e3211f1b053b",
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
              "id": "297f5070-6943-466e-8390-b35c9904a680"
            }
          ]
        },
        {
          "id": "09b2dbef-71a1-4eea-8686-254dd50bffcb",
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
              "id": "7d2cab45-31d6-4385-b22b-2ddcaaee035f"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "230a418d-663f-4bd8-a325-3aad6aaff3cb",
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
              "id": "a5807580-e1e3-4033-ae69-611c7893b58c"
            }
          ]
        },
        {
          "id": "c548a30d-7ddc-4ff2-865a-305e3a7e0c9a",
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
              "id": "ba0af13e-1212-42a2-90aa-50894208d179"
            }
          ]
        },
        {
          "id": "bd862c12-1403-4515-9f67-86f207e8da49",
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
              "id": "045fba04-4b6f-45e9-ae8a-4882f73c1512"
            }
          ]
        },
        {
          "id": "cdabc3be-c485-46da-a7d8-b8d964d75c95",
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
              "id": "0446d3f4-85b8-4fae-be1c-50c1a4f91da6"
            }
          ]
        },
        {
          "id": "4d8d2aea-1834-4b4d-a7dc-6afc717f7cdd",
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
              "id": "36c8d34c-5d19-4823-b430-d6024bfa5dca"
            }
          ]
        },
        {
          "id": "61517c8a-c2de-4b1b-a6ac-3b19d4ffcba6",
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
              "id": "cefa077c-00aa-4fb9-843b-fd62ddba9ad7"
            }
          ]
        },
        {
          "id": "dabfc83c-0d2e-414b-a899-579374249a5e",
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
              "id": "9a2cedfb-ff1e-4b5f-aeb6-a6e9fe51806b"
            }
          ]
        },
        {
          "id": "e5b95986-efe2-48d3-8525-b7bae962cb4d",
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
              "id": "586e58c8-c23e-41fa-8989-cdc6b281d901"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "e5841700-ec77-4bf2-abe0-51baa4577f4a",
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
              "id": "1b013628-2064-48ee-a1ec-7e457e0ec83f"
            }
          ]
        },
        {
          "id": "88ad84b3-5926-4c00-8528-fea1775a27ff",
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
              "id": "9daa125c-994a-46d2-b7a2-088aeb4f8901"
            }
          ]
        },
        {
          "id": "e0704865-abd4-46a8-8fd2-f18a0fbad2da",
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
              "id": "922a3a92-644f-492a-896f-3c5a833b32f1"
            }
          ]
        },
        {
          "id": "dc89eee1-d915-4a7b-9f0f-46218ccefa61",
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
              "id": "56c014ef-46cb-418a-a297-17b4c1457850"
            }
          ]
        },
        {
          "id": "a96ca4d8-3080-441b-b408-7153aa876c18",
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
              "id": "5c3d510d-0612-43d0-aadf-993347a78dec"
            }
          ]
        },
        {
          "id": "d130cda7-c478-4ddc-ae2c-13e1c38a6eb1",
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
              "id": "993c2890-3e06-4cf0-8db3-f1b2fe668859"
            }
          ]
        },
        {
          "id": "8d565aa9-22cf-46ee-bb5d-891949ccf932",
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
              "id": "9e1464aa-4b81-49d3-b26c-84b1b8d5e418"
            }
          ]
        }
      ]
    }
  ]
}