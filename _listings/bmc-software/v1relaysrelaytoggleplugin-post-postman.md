{
  "info": {
    "name": "BMC Software API Toggle relay plugin",
    "_postman_id": "640c4c23-566b-4e73-b88f-875cee48391f",
    "description": "Sets a relay plugin to be disabled or enabled",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "b20dce8e-7198-402d-988e-3e6cdcd21a21",
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
              "id": "60af2912-6acd-466d-a8bb-0116573a93aa"
            }
          ]
        },
        {
          "id": "2f6382d7-11d4-41d0-8e47-da11b4591bff",
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
              "id": "562a3c2f-18c6-4aef-9f36-75707757b6f6"
            }
          ]
        },
        {
          "id": "417ff69a-d538-4b4c-a89c-012fde63c29e",
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
              "id": "bc0a3c9f-2596-445c-b1c1-51b6ff53f829"
            }
          ]
        },
        {
          "id": "92a58851-e0f4-4290-ab40-cbdb3cb9787d",
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
              "id": "323f1082-c40f-4c67-8f38-e00a4f579251"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "38fad303-17ae-45b8-a6c1-ce1a685c8870",
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
              "id": "d3f26399-5f0c-4446-95a5-8a6137609930"
            }
          ]
        },
        {
          "id": "6275d7ce-eaf6-45b9-a8c6-f6ce58f492d1",
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
              "id": "ff824009-791d-4c1f-9107-d9b30962def2"
            }
          ]
        },
        {
          "id": "ce1f6a87-a558-473f-ac99-73a0911243b3",
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
              "id": "6cbc4d3e-8fa4-428c-8b5a-ffa44debd197"
            }
          ]
        },
        {
          "id": "c93ac2d0-ea0a-4523-97e6-8a83a47a1f5e",
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
              "id": "0384f2d8-19ea-4ff8-b3b9-2d5b1adfb142"
            }
          ]
        },
        {
          "id": "fe621c99-01bd-45f0-beec-368bf3294740",
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
              "id": "79da38a1-da08-4084-9932-2a846479f633"
            }
          ]
        },
        {
          "id": "6d4230ca-d6cd-4391-9187-e400ed0d3696",
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
              "id": "3512c70a-27b2-4720-a717-9fb199449bbb"
            }
          ]
        },
        {
          "id": "452e9ffb-3d7c-4853-bff0-6cd2a7337f1c",
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
              "id": "734844d2-c700-46b9-be8f-cb9967cab246"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "9913369b-9b1d-46b4-a71f-4e0f32a87e98",
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
              "id": "289a995d-acf5-42bc-85e4-0a64a6014c67"
            }
          ]
        },
        {
          "id": "f9bb6703-6507-4426-b218-4d758bb8eb5d",
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
              "id": "364e98e3-7afa-49a9-ae81-eecb831bd168"
            }
          ]
        },
        {
          "id": "e2fe5fbb-20a1-4361-b99c-20eea39a895b",
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
              "id": "68cb20e7-969d-4208-97c8-0b56e3ecd398"
            }
          ]
        },
        {
          "id": "520f2770-f938-4c7d-a84b-fa93e7705b0f",
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
              "id": "6833e5e1-48cd-4ce9-b601-418443197209"
            }
          ]
        },
        {
          "id": "db719618-a66f-4d8b-a818-27d18a308eed",
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
              "id": "7ceebc50-f71f-4a8d-bae6-0a3223ee4ead"
            }
          ]
        },
        {
          "id": "26b591a8-36e8-4b81-89c8-5d4fb6f72e21",
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
              "id": "e1a3f4c3-60ac-4d89-9151-97d6a536ebb4"
            }
          ]
        },
        {
          "id": "be625250-350e-49ca-8139-3a117dd73c0b",
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
              "id": "fbe57542-9c2c-420d-9327-1486462e1c9d"
            }
          ]
        },
        {
          "id": "6d9d9a95-63c2-43a8-a241-d9de9b51ffbf",
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
              "id": "004cf0a5-1ced-485b-a00a-d50d00bc0a61"
            }
          ]
        },
        {
          "id": "295265db-6c04-431f-84b7-12f10517cc44",
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
              "id": "d26fe747-e503-4b62-93c2-f634540670a4"
            }
          ]
        },
        {
          "id": "edfe8a27-5a8a-4119-9376-a443b30889c2",
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
              "id": "9d076849-c88e-45cf-b677-9b485bdf1f81"
            }
          ]
        },
        {
          "id": "ea9a0a58-af93-473c-bbeb-2f44b61b11eb",
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
              "id": "122293cf-730c-4b73-bfc1-a0c54c36a5c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "d89f32e4-5e7a-4b17-99fe-72f25874dad4",
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
              "id": "c43c84a7-56a1-4170-bc0c-bf46180c0844"
            }
          ]
        },
        {
          "id": "4622fba6-d889-41b5-8d76-c1ff8f623a30",
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
              "id": "33ff2a13-80cc-405b-9607-153608126a26"
            }
          ]
        },
        {
          "id": "aea7e51c-bc89-4878-ad13-7310a5244476",
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
              "id": "2f387d92-e90b-4c07-a02d-833cdfed7863"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "6f664ea3-34f2-4105-87cb-0a01b76d39da",
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
              "id": "86f3291d-860e-4dbf-b4d0-b00e808bece3"
            }
          ]
        },
        {
          "id": "d7419cc9-1b84-4772-8d8d-73394c3c792f",
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
              "id": "a1eec595-d5d7-4c81-97a6-47496e38ca8f"
            }
          ]
        },
        {
          "id": "69d99146-24a7-40de-83ee-75a110298de0",
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
              "id": "ec9231ef-ed27-46b9-baf7-2061c355627a"
            }
          ]
        },
        {
          "id": "b63f88f4-de6b-4d85-aaa2-a95657e9f866",
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
              "id": "112a1df1-49e0-4caf-918e-c043a887907f"
            }
          ]
        },
        {
          "id": "fdf662e5-dfc2-4330-bd09-891af34d02dd",
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
              "id": "62aa7b22-5afe-4590-a2e3-54acc4812950"
            }
          ]
        },
        {
          "id": "34fc54ff-33b9-40fb-b539-583018b04d48",
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
              "id": "0f242ae8-8b3b-4417-a4eb-6b73830d54b9"
            }
          ]
        },
        {
          "id": "09a227a8-bdf0-4a9d-9399-6e6b13ca6d6e",
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
              "id": "9f22f623-1d94-4ce2-8cf6-36265e9ded1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "282829af-057d-4cde-a7fc-319e9b061850",
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
              "id": "31f99595-86ae-4954-92ed-7f497e8c9028"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "cc524357-fa3c-47ef-8ade-f6f08159cad7",
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
              "id": "c8751491-23a3-4744-932f-389aaa9b0e82"
            }
          ]
        },
        {
          "id": "df07a39e-bdbb-4056-a390-3f9545b224fa",
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
              "id": "6b091c6d-b4b2-4137-b1fe-b36aaf4fae21"
            }
          ]
        },
        {
          "id": "36bacad2-4a52-45c0-a021-d6e1c12153b0",
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
              "id": "5c8dea13-242a-4ab6-91eb-31f357349d93"
            }
          ]
        },
        {
          "id": "46eb7454-3075-4833-b347-7ec6af692e9b",
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
              "id": "87f0e922-365c-4b2d-af40-2a1634aa64b2"
            }
          ]
        },
        {
          "id": "d8529fd6-4dde-430f-9bd2-f83c17dcba6e",
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
              "id": "012d9043-e216-496a-b9af-73883322b9fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "7ba32ff5-8d65-427d-a8d7-a7aa786d3037",
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
              "id": "440e688a-d880-4467-b313-a1f5540d0394"
            }
          ]
        },
        {
          "id": "6a243bca-7711-4dfd-b30b-c5cdb97b92dd",
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
              "id": "9869685a-2c0c-4c3b-a5f5-6c61391e2c49"
            }
          ]
        },
        {
          "id": "4cae8167-6d3a-446b-91ab-3b88b16e7138",
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
              "id": "963d3483-5594-419f-8771-3b8b987734ad"
            }
          ]
        },
        {
          "id": "3a68b399-a06b-4187-bf7e-f2bdc9880605",
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
              "id": "257c324d-f068-435c-8650-dd42c825b17d"
            }
          ]
        },
        {
          "id": "162a11c2-adad-444f-86d9-19c61a407108",
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
              "id": "8793be77-a38a-4d66-bb0a-1ae2a64df039"
            }
          ]
        },
        {
          "id": "0f14796b-2c5e-4123-a6e7-94eb80481fc0",
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
              "id": "d6f1743c-f1ae-4266-a687-195b70baab17"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "34c4c889-5f60-470e-9407-789a4e50d2a7",
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
              "id": "51fb9c7b-5d43-497b-b87a-beccf59345d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "757c20a3-bee3-4717-9237-022b22615737",
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
              "id": "b961d997-ab20-4635-b16c-c4732eebbf42"
            }
          ]
        },
        {
          "id": "823a1370-63f8-4407-8f80-9a478f10e76f",
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
              "id": "6e0bfecb-fa71-4b97-a94c-c9019b4b0a83"
            }
          ]
        },
        {
          "id": "1c7a54f1-c540-41d4-99c7-5ec6ff9d57ab",
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
              "id": "e132302a-a5ba-43f6-b4b4-8ea6688d9e7e"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "80564601-b6b4-41bf-9b68-0499de4324ce",
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
              "id": "ec184beb-7fd2-450e-9683-9cdc51480566"
            }
          ]
        },
        {
          "id": "82d22c41-e7c4-4bd1-9c04-f18ebd5d6f6e",
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
              "id": "0bf86947-74e7-49d9-8c25-7c76e4757edf"
            }
          ]
        },
        {
          "id": "ae52da71-f908-4ec3-b188-07a0ab5bd3fd",
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
              "id": "13b7ed2f-4489-4cef-9aff-cd9fa4071df9"
            }
          ]
        },
        {
          "id": "34267b9f-e1b0-4847-becb-1b164a887e24",
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
              "id": "16bffd1a-b1a0-4a36-aeea-cff6e30c5c9b"
            }
          ]
        },
        {
          "id": "222fb886-686f-496c-b9d2-49a219005a85",
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
              "id": "cd07152a-a9c5-450a-8c8e-9cc5e6cf7b9c"
            }
          ]
        },
        {
          "id": "cb652a74-c1ce-4f29-9681-e5c8fcc96280",
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
              "id": "a9730e88-c5cb-4c30-80b9-723dd13ccb71"
            }
          ]
        },
        {
          "id": "6df1bf3a-4236-4454-ae8e-b32c6bca4015",
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
              "id": "863603d1-aa49-4b55-b253-9f78cf23f2fe"
            }
          ]
        },
        {
          "id": "ee8abbcf-1b77-40b6-8d10-3b747fb53e95",
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
              "id": "4ca364dd-c005-471f-b09d-fc96a141bdc7"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "70374c9c-69ee-44c4-8376-96955655228e",
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
              "id": "ff7210ce-9e23-415e-b1c1-66bcf90e79d6"
            }
          ]
        },
        {
          "id": "0d2328d6-2deb-4f18-aa16-d457f11ab825",
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
              "id": "ebad7a88-c0d1-4308-aefb-b5d0a9c1be74"
            }
          ]
        },
        {
          "id": "cfab1661-4431-446a-a357-81c40131672a",
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
              "id": "2347b1de-9712-493c-8dec-9800e868fa4b"
            }
          ]
        },
        {
          "id": "de600b57-f270-4f0c-ab83-59f4059a8d9b",
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
              "id": "1901915e-03aa-42e6-ad0b-e373c2f8d6ed"
            }
          ]
        },
        {
          "id": "f19082f1-a6e1-4178-8cea-772c2764633e",
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
              "id": "d8163541-3677-46ac-a752-41f978cfad4c"
            }
          ]
        },
        {
          "id": "de791c41-75c0-4986-bb26-b44f0a465990",
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
              "id": "828029dc-5a1d-4bce-ba87-983793987cdb"
            }
          ]
        }
      ]
    }
  ]
}