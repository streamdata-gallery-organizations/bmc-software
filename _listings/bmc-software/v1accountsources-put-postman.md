{
  "info": {
    "name": "BMC Software API Set source metadata",
    "_postman_id": "cfde5aa1-ed62-446b-861d-76ee5498c3f1",
    "description": "Sets one or more source metadata",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "a71a4b21-cd7c-446b-8ce3-47a5e7e83daa",
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
              "id": "523ca763-4573-4103-91d3-c433bc4d95da"
            }
          ]
        },
        {
          "id": "65be65ae-71d1-4551-a71a-d681cf85a29c",
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
              "id": "2da61ea8-b6c1-4db2-b2ac-b8fb83168729"
            }
          ]
        },
        {
          "id": "e5f54ed9-7574-4c0d-a1d9-5192fe2efa45",
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
              "id": "6ba8c2f4-b0d6-4b9d-b9c4-7d9ec3521e5c"
            }
          ]
        },
        {
          "id": "2376ad72-5c84-4319-b05c-19e4ec6353dc",
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
              "id": "71a8053d-384a-467e-9160-030f240016cb"
            }
          ]
        },
        {
          "id": "e640483a-eaa1-49a0-b49d-52843bf3ee63",
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
              "id": "ed9b0c6d-2f72-46c6-b3b0-fe56ef73c29a"
            }
          ]
        },
        {
          "id": "30fcce79-0e98-4e29-bec7-bf8d864fd4c3",
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
              "id": "918d1582-8653-49c5-b7d6-b07c0271a40a"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "e1e359bb-162b-4694-9f77-f7fcc586cd76",
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
              "id": "33adb7bc-2a68-402c-832f-5a07cf9c6135"
            }
          ]
        },
        {
          "id": "76347b17-e307-4b73-af55-8e9cdf25393d",
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
              "id": "63bdc726-c5da-48af-8cfa-1e47a024b1d9"
            }
          ]
        },
        {
          "id": "ed134e83-7a10-498c-8ec2-f2617e32ee67",
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
              "id": "e71ae673-5f9d-4ea8-9dba-4f750d7082f2"
            }
          ]
        },
        {
          "id": "af71cd55-6119-4198-84d4-31ed64a25f2e",
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
              "id": "db99c63a-dcd8-4461-a164-529753ff4368"
            }
          ]
        },
        {
          "id": "1c1c588f-5cee-4516-85ab-66bfde17193e",
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
              "id": "5782d74c-745d-4b9e-b71c-c4d1f55964eb"
            }
          ]
        },
        {
          "id": "f636094a-ffb9-444c-bad4-9c24bf1e6482",
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
              "id": "49134a6c-ac63-4d54-b28a-1f386d611d9c"
            }
          ]
        },
        {
          "id": "eaf98ad9-f98f-479a-a247-eb0cbebdec83",
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
              "id": "5e5b448d-f656-4593-888c-7c1131264dbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "858aec1b-5f3b-481c-852a-ded493d9d03d",
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
              "id": "8aff1b77-f87e-497f-8c24-48d4583f6cf0"
            }
          ]
        },
        {
          "id": "c3bae797-ef51-4de0-81d3-17e2812df55f",
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
              "id": "50aca19d-6805-49ff-b2e4-a50a5d9529ca"
            }
          ]
        },
        {
          "id": "4f6dc9b2-0a6d-48b3-9db9-0213abbd815f",
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
              "id": "9718e041-c64d-4a63-a529-78fccc0eeddf"
            }
          ]
        },
        {
          "id": "1bac085c-8e4e-4f7e-aaf6-c1eb1cc97e86",
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
              "id": "f016495a-5236-4517-aba6-c2ecb398d90e"
            }
          ]
        },
        {
          "id": "1c2160f7-d142-4f05-817b-e650cb5fde43",
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
              "id": "e3402673-0475-472f-ab2c-e42cc5a4933a"
            }
          ]
        },
        {
          "id": "c8342a00-7cc3-4eb3-8f26-16a65476d0b5",
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
              "id": "8a6facdf-5c5c-434d-8efd-01dccb911316"
            }
          ]
        },
        {
          "id": "0564e013-c7ab-41c0-b3c4-e4ade1b9aedf",
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
              "id": "3eb9f65c-5eb8-4363-9dc8-5780097f13ff"
            }
          ]
        },
        {
          "id": "39a4c3c8-b495-4584-be58-d577ee9e8bac",
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
              "id": "105bd1a9-a29c-4b4c-b269-a79756968ee4"
            }
          ]
        },
        {
          "id": "4fbe47dc-e509-453d-979f-ea35f552b8b0",
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
              "id": "d499512c-756a-4969-9322-dbf4396c4f71"
            }
          ]
        },
        {
          "id": "b5f5d055-cf5b-4a17-84d1-5572266b2a84",
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
              "id": "4d8ffb5a-1542-4cb9-bd0e-111d951fb3d1"
            }
          ]
        },
        {
          "id": "3d7931e7-2299-4564-81a0-4c9d0defe3bf",
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
              "id": "717dbcd1-8948-4a9f-84ac-166e9d4e0547"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "ecc5b340-3c3e-47f4-8020-e988bf95e131",
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
              "id": "dfd5ae98-5e9d-4ecd-99dc-d61943d9f884"
            }
          ]
        },
        {
          "id": "cb8f0375-4b40-4c8c-ba84-6af750a43f86",
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
              "id": "5922b922-e074-470d-9017-3d632d47e29f"
            }
          ]
        },
        {
          "id": "b110f11a-9903-4832-b4b5-3b621fb61727",
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
              "id": "f73051f9-2adb-4dc9-866b-020c2d601637"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "94cff69b-76b5-491b-851f-8527a2e45745",
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
              "id": "0e9b3d27-330b-4f61-9143-8ffdfff8b2c7"
            }
          ]
        },
        {
          "id": "977d712b-78c0-40c8-9ba9-a955e608bebf",
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
              "id": "2b1f66bf-cacd-4fd2-a875-f8ecd3101794"
            }
          ]
        },
        {
          "id": "2def6496-86ff-4f46-8c31-ec24c06ffe57",
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
              "id": "ef41d74a-2c72-494d-80e1-4f87de842091"
            }
          ]
        },
        {
          "id": "de663eb3-b88a-4f11-8ab3-a20f15fa88f8",
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
              "id": "1c57b889-2acf-4d76-89e0-342143542a73"
            }
          ]
        },
        {
          "id": "d1711883-e88b-4496-b881-23eee8f6a712",
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
              "id": "3fb18539-6a88-4de7-8db9-f7988e709645"
            }
          ]
        },
        {
          "id": "0d9c21b1-11b4-491d-9ded-480ab098beeb",
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
              "id": "53437ac0-6fde-45e0-854a-03e38c291ef3"
            }
          ]
        },
        {
          "id": "1c78db59-0cbc-4cc2-aff3-69b5da57f761",
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
              "id": "3f6d8920-09e3-4efe-b736-9e6ee55180aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "2b902950-1abc-49f7-ad7f-f514b78e4b97",
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
              "id": "46b82f5b-dc16-44ba-80e5-f5559ff1b9e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "18034c4b-1499-4544-885a-c961f30023d1",
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
              "id": "1479db29-bec7-4f42-842b-96d4bdd79181"
            }
          ]
        },
        {
          "id": "74d58824-e509-46b9-80fb-f73b5d4273ef",
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
              "id": "ed5343a8-9809-469e-93b6-e9fd0133fd7d"
            }
          ]
        },
        {
          "id": "a7c423b1-aff6-45c1-bf62-9ac0125a85b9",
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
              "id": "8c133b8e-c964-43c6-bbee-86c45f514c2a"
            }
          ]
        },
        {
          "id": "f25c5e5c-7c8f-4f39-b056-836bf21fa0c7",
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
              "id": "f373a6a2-ab36-4b73-be57-763631088edf"
            }
          ]
        },
        {
          "id": "ca0c35a0-f794-423f-806b-017b42f82a13",
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
              "id": "c5907441-5acc-44c7-a4a0-aaeac8c9f80d"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "822abcab-1573-4fb6-9fc0-d8e9713366eb",
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
              "id": "c48f447b-24c9-4ae7-b746-eb0bb4c278bc"
            }
          ]
        },
        {
          "id": "7d7eaf82-0609-4d1e-bf89-0a84d8f640cf",
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
              "id": "a6531e61-bf22-4ce1-93ec-d6b07e6f8938"
            }
          ]
        },
        {
          "id": "63c609d4-6e14-4d89-b491-eb9859c646be",
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
              "id": "6ae56cf8-1d5b-477f-9737-86a3a12a7bfe"
            }
          ]
        },
        {
          "id": "2c7b4640-c40b-4fde-9a3a-e0bb0ef45e8e",
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
              "id": "2cd202b1-244e-4184-9eee-71e98108e294"
            }
          ]
        },
        {
          "id": "9d099c34-e4cd-42bd-93d3-5650573b842f",
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
              "id": "fa569728-9a49-4ed3-8408-3826dff82ce7"
            }
          ]
        },
        {
          "id": "030954db-427c-488c-b389-70d1fc599f03",
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
              "id": "9d51aacd-eb79-4f7c-8e1d-fcc55cfb6e46"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "0989987d-fdd9-4d22-b4ba-4db867e7e144",
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
              "id": "279d435a-eed9-4387-b7a2-51df951a5437"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "7f19049e-cdf2-4d3b-aaed-fd13835d1e54",
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
              "id": "45b96429-72c5-4741-9117-c5c0d0c980f5"
            }
          ]
        },
        {
          "id": "2806f53e-c418-47d8-bc3e-a70e07d24430",
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
              "id": "97104262-f07c-4f3e-8a8f-06f5dc5664fe"
            }
          ]
        },
        {
          "id": "1c30b88f-c9c3-4c6e-9b4d-22f655cea15e",
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
              "id": "3c3e9b61-29f1-4e8b-b507-b652610acff5"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "16575d14-1c8a-4ab2-b622-edfc12c43f49",
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
              "id": "8b898d1a-5b67-47cd-a56c-6d74be97f151"
            }
          ]
        },
        {
          "id": "3b2db964-a0ec-485a-98d5-ada53c4d635b",
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
              "id": "a2e2ef74-bca6-4f28-b125-d79cf4ad7118"
            }
          ]
        },
        {
          "id": "2c56431d-84de-45be-ba16-7d72312092f1",
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
              "id": "0d3c2c2a-ee3c-44f0-a542-083c293cf4d4"
            }
          ]
        },
        {
          "id": "02ed99e7-e406-49b6-afd2-6a03518f0f86",
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
              "id": "82c90d57-61e4-4006-95c1-ee74b58f8c43"
            }
          ]
        },
        {
          "id": "2e93629f-6b32-4b60-9c42-c8e4d224fe1e",
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
              "id": "1de5ae7a-5600-4066-8e70-6ecb28551376"
            }
          ]
        },
        {
          "id": "eac8993a-255c-4162-82af-66fe85502168",
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
              "id": "7d5dbb45-ce12-4b4c-8168-b424e0ced7d0"
            }
          ]
        },
        {
          "id": "0e65a135-f960-4141-933b-0e14211ae848",
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
              "id": "08287fc2-4aba-4bcf-bdfe-96ffbd95606a"
            }
          ]
        },
        {
          "id": "ed8d4320-f9a8-4e4d-958e-b51f8dfe74da",
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
              "id": "d5327cd4-9c34-4b37-a30b-3f9ded6bb4a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "1cec4841-62c9-4354-a279-22bf2f570eef",
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
              "id": "f3608398-b7ab-4905-8a0f-b681473db210"
            }
          ]
        },
        {
          "id": "862f4224-ac9d-4934-bf5a-88d62bfa9bc8",
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
              "id": "5430d6cd-97fb-4ad5-98ab-c0e718ce06f9"
            }
          ]
        },
        {
          "id": "e66f542e-d0fb-4266-b700-d83aed7934f9",
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
              "id": "7dd66926-7521-4319-9c51-250cf9cd7ed3"
            }
          ]
        },
        {
          "id": "469414ed-c932-41e9-93aa-e58b682b8ae4",
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
              "id": "5fddea4b-a0e1-4dcd-9fd4-bbb910c13c1d"
            }
          ]
        },
        {
          "id": "6165020d-d2eb-4d5f-9a6a-f600750d4bd5",
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
              "id": "5c6f30b4-aad5-43a9-912d-1a2c538f8e7c"
            }
          ]
        },
        {
          "id": "82fc15d3-60da-4fbc-9250-233834a5753f",
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
              "id": "3988649f-deda-4643-b629-400c9022a002"
            }
          ]
        },
        {
          "id": "41cabb00-6459-43a5-aa0c-c42e24915599",
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
              "id": "6d67d69f-2788-4cb6-a2d1-84b9478def9f"
            }
          ]
        },
        {
          "id": "76fee201-33bd-44a5-8c8b-b24c5b7b5858",
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
              "id": "5814b3bc-d479-4252-80ac-aa106ef0b875"
            }
          ]
        },
        {
          "id": "9502dfa1-2990-4932-bbbe-f907fa2dc53f",
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
              "id": "bf2f1d0e-a67a-4682-b035-2f8ab377e3dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Sources",
      "item": [
        {
          "id": "cf759c92-28a2-4469-9765-1ce79bfd1056",
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
              "id": "eb38df98-d5e9-45bf-8dfe-ae9443dfa488"
            }
          ]
        }
      ]
    }
  ]
}