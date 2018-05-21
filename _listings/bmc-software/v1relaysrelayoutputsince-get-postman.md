{
  "info": {
    "name": "BMC Software API Get relay output",
    "_postman_id": "8665d008-dc03-4276-9778-331fc7a580c3",
    "description": "Queries for relay output messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "d9f1aba5-a5ae-4445-aef8-07710f2f9afa",
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
              "id": "f189d6be-0c9c-4757-94f2-a3c4529dab18"
            }
          ]
        },
        {
          "id": "ec6d2d66-7426-4b82-b2a6-43259df68a16",
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
              "id": "268581c7-3692-4d43-822c-2aaee095032b"
            }
          ]
        },
        {
          "id": "fb098782-73a7-4e7f-be30-30d7c21e9723",
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
              "id": "9ac1b269-e3a4-47ff-a62e-c340e3bfa5f6"
            }
          ]
        },
        {
          "id": "73c9c740-d91b-441a-b5c8-e6e2a10d6aa2",
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
              "id": "47434cf1-6b6c-4652-82c3-bc3c6581a6b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "8fd91823-26e0-45c8-a5d3-150d96c8afd2",
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
              "id": "0706b815-c515-4b38-92fd-5a64ca190ad2"
            }
          ]
        },
        {
          "id": "1c80cd2d-02a5-46b7-99d7-4d843cfab0dd",
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
              "id": "783a297f-88b1-432f-99a6-a0c70b73da23"
            }
          ]
        },
        {
          "id": "e5a61125-09e5-4a82-832e-a125efabca64",
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
              "id": "1a640d38-9d86-4ce1-8022-76fe34590f48"
            }
          ]
        },
        {
          "id": "00fa9ac7-db41-4157-b6d3-9598caf10b0a",
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
              "id": "85113187-ab0c-4018-8a1d-ed13ce2ce75b"
            }
          ]
        },
        {
          "id": "61a619a3-be96-4a05-99f9-2bf437aa6829",
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
              "id": "a728597e-71b6-4ed0-9d4c-e0fadb73ac77"
            }
          ]
        },
        {
          "id": "b198d08b-87a7-48fa-ad52-51c275b43337",
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
              "id": "0fe4f612-19c5-4e3e-93e4-15ad7ecca3f9"
            }
          ]
        },
        {
          "id": "7b0ce378-9384-4d12-ad2f-912ff01b74c6",
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
              "id": "958325e7-06ac-4005-9aab-e87a4b5aad58"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "b2f8ff93-398d-4215-835a-67b3d7699c83",
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
              "id": "3c1acab3-b9e6-47cc-bee3-4a5ade8d0a53"
            }
          ]
        },
        {
          "id": "9e954272-7453-485e-ab97-b8075a697289",
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
              "id": "edcc2090-3b14-4a41-bc49-ed401fca63fa"
            }
          ]
        },
        {
          "id": "8ce76b89-fa44-4b61-8fd8-4f712faf09ce",
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
              "id": "869538c9-17de-46ad-995c-41f0874ea549"
            }
          ]
        },
        {
          "id": "4dc9a1b9-5bc5-400a-bb98-aa58f61fd25b",
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
              "id": "29d61932-9ba8-4e55-a862-b684c47b81a8"
            }
          ]
        },
        {
          "id": "3a4a0a60-ccad-47f5-8f6b-d491348b46e1",
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
              "id": "af8794c8-1e7d-4300-b52e-6693c9229272"
            }
          ]
        },
        {
          "id": "fd708987-0dce-482f-92a8-f8aa770c6fc3",
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
              "id": "b2a414eb-c003-476c-8c67-176b1932f7b1"
            }
          ]
        },
        {
          "id": "5d881bc2-0959-441f-be39-955263226126",
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
              "id": "3d4027e7-dc5a-43a5-beb3-6f4ee6d711d8"
            }
          ]
        },
        {
          "id": "beb303b7-31ae-4522-81c1-ef6d8081eb48",
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
              "id": "02026ba0-c9ac-43be-b01e-c888792cee78"
            }
          ]
        },
        {
          "id": "82deea3e-8f6a-497c-a7e1-0b7be1264f8c",
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
              "id": "854dcb0d-cb94-4dff-88ef-6ceae5edd1ca"
            }
          ]
        },
        {
          "id": "8708048d-7b33-4cb8-aabc-4adb615e68f4",
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
              "id": "aafd3a97-e6e4-4fd9-affb-f5f73562a3a9"
            }
          ]
        },
        {
          "id": "2f00c5a2-4bf5-45d5-b983-7aeccb17f35a",
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
              "id": "5ccc5ef0-919a-4b62-ae92-9c78af39b7ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "92402a48-3b12-434c-9b2d-c3ee564fde22",
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
              "id": "360cdf77-4ddd-4ab2-99ea-e929cfe351c9"
            }
          ]
        },
        {
          "id": "6ece5420-ac3c-4188-b0fe-d57430d07df8",
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
              "id": "7a844574-f364-4e0e-ae97-f0044b418f7a"
            }
          ]
        },
        {
          "id": "b26fda5e-a6d2-4a46-a1cd-113b69e5c71f",
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
              "id": "a10113fe-0825-4c20-a6ce-5397f213b57e"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "e0766f3e-b92c-4eb1-9f34-031db3c05dca",
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
              "id": "2e0e529a-24bd-45a1-b821-8aa2a63b0a67"
            }
          ]
        },
        {
          "id": "dc57d127-fdc1-4e9c-bc97-ae35cd54c208",
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
              "id": "57843296-c7c9-4253-a02d-8c53b95ef2c7"
            }
          ]
        },
        {
          "id": "3fdbb21b-1fbd-430b-b3d1-cb00fb406a7c",
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
              "id": "027e1c63-d47e-4502-905a-08b27f8ff948"
            }
          ]
        },
        {
          "id": "0fd1ad1b-3406-42d7-8e95-2dc1a434afbe",
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
              "id": "a891ebae-da41-4aef-9ba7-71d7fdfe53d1"
            }
          ]
        },
        {
          "id": "0fccb5c6-8259-47f9-ba69-be3b6702c14e",
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
              "id": "94b887e4-be73-43ae-a920-6c83afc4146a"
            }
          ]
        },
        {
          "id": "d9292e8c-5e76-496c-862d-56aa5ab83f37",
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
              "id": "ce45c257-8057-479d-af24-4e8e2a85d2d3"
            }
          ]
        },
        {
          "id": "0ce2d228-1f5f-4c26-974e-14775796a613",
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
              "id": "74e74ae5-faf1-4212-8cdf-38bc63bb2479"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "4d8cf059-c88b-410c-955b-fb97d8c4eb53",
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
              "id": "32036a3d-583f-4262-bcdf-24cf1250157b"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "52631b54-0147-400e-b6aa-21d54c15ba23",
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
              "id": "c22dc418-1960-4309-a08e-0eaef4be67c1"
            }
          ]
        },
        {
          "id": "ad886f7f-74c4-4f78-bc16-a57cd6728fd7",
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
              "id": "c94566a1-1e27-4f28-b6ac-26d49c1fea4b"
            }
          ]
        },
        {
          "id": "01dfa542-53a2-4ad1-b737-a0b6ab36e70e",
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
              "id": "9a78a8a6-c476-4e68-9830-1a016248e759"
            }
          ]
        },
        {
          "id": "8696d65a-de29-4c48-b7db-a7503671dd5b",
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
              "id": "fc779b9f-a46e-47de-add9-84b768a18130"
            }
          ]
        },
        {
          "id": "2f6366a9-7c2d-452e-9d53-4c31909263f4",
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
              "id": "0a1786fc-5641-4f44-844b-3732599bad34"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "0bce5d49-4a6e-46da-8985-dc45dee56ccf",
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
              "id": "f88e63dd-af76-485e-93f1-3192a89d0672"
            }
          ]
        },
        {
          "id": "7f3b22ef-c344-4a6c-9278-0eed8dabf793",
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
              "id": "f274e647-b822-45be-98a6-6231da6455f8"
            }
          ]
        },
        {
          "id": "0e041a85-5abc-4ca9-87e7-5a8be44a5301",
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
              "id": "79fa391f-1f40-45d9-a3c4-c0731780aa44"
            }
          ]
        },
        {
          "id": "0b49fb58-eab5-4f67-9172-ba4de9de6c66",
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
              "id": "0ca950f0-a687-4825-99fa-e41ebab6ce7c"
            }
          ]
        },
        {
          "id": "848f9549-cbd3-463d-973b-2eaee9267b7f",
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
              "id": "0b11568a-e672-4fb2-8c93-d2b5a0a2af8a"
            }
          ]
        },
        {
          "id": "2c39474e-b9d3-49d7-a553-d4433102b931",
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
              "id": "ee611f46-16c8-481d-8a4f-161bdf2437e8"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "0efbf3bb-e9b4-45cb-ac25-0ab7a91b0006",
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
              "id": "3c3827a1-367a-4dd9-ad31-cf7ff3d7b728"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "de095564-307a-4763-bb62-a753e8b3b122",
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
              "id": "476895d2-88be-4143-9aff-73a4f2b977fd"
            }
          ]
        },
        {
          "id": "93e13629-f132-4811-b99c-a84f2ad27ad7",
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
              "id": "f14c8938-4035-4b31-b6fc-1037dcdbca14"
            }
          ]
        },
        {
          "id": "e6dae776-ee8d-4324-a52b-37a77f497633",
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
              "id": "f155b9fc-3441-46a8-b265-ced4c90cf876"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "1cbadac3-4565-497b-b0ee-874aa70e9064",
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
              "id": "c41d296c-8859-4590-bb36-f18b0c9781e8"
            }
          ]
        },
        {
          "id": "ff06f678-4560-4a46-a54a-affc16b87437",
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
              "id": "7a04fd43-bbd8-44e4-8d47-6eba27719af2"
            }
          ]
        },
        {
          "id": "12e7cb48-b275-4343-b3f6-0d25e37ebba9",
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
              "id": "ddebeb02-dfe4-4f3a-942c-641f9e3c1c23"
            }
          ]
        },
        {
          "id": "89d925ef-e802-4875-a7c4-e6bc00a8634d",
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
              "id": "290b9ef6-8648-4391-908d-a72f512c5746"
            }
          ]
        },
        {
          "id": "5649eeec-c5ca-4fe8-a6f9-2265cd9ba19b",
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
              "id": "1c8c8643-e7e6-4591-bb9a-4fcf32d5917e"
            }
          ]
        },
        {
          "id": "3a6837c9-1a3a-4417-84ae-58190300fbee",
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
              "id": "8137525d-faad-4a70-b759-2adae4fb3326"
            }
          ]
        },
        {
          "id": "3688ea8a-2bfa-4d1f-8294-e9ca6860eb91",
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
              "id": "80e87268-ab87-4603-9d9b-834aaa37b017"
            }
          ]
        },
        {
          "id": "ab967eaf-0540-4c67-8017-6b24d886f1b4",
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
              "id": "190a4812-3689-4ec0-af49-2cd42d4e6367"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "dc4ab4e8-4e07-4787-a29e-ea88753d53bc",
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
              "id": "2e47ac96-c9db-491b-bac1-275fac31d453"
            }
          ]
        },
        {
          "id": "c2e2dc53-718c-4e69-acc7-d5ae40b7dc4b",
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
              "id": "11cc06f2-33cd-42c6-a54b-8d8b98c76d8b"
            }
          ]
        },
        {
          "id": "9a3d7a15-29e5-4abd-89f3-7c575747df5c",
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
              "id": "7accdab7-030e-44b7-9d5f-7235aba3c8ef"
            }
          ]
        },
        {
          "id": "2bab5f41-0c35-4fa6-a59a-75da6bda3867",
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
              "id": "1c01eb71-a48e-4999-a8a1-e4f5b686083a"
            }
          ]
        },
        {
          "id": "a8d0584c-abd1-4a51-b168-6f3b53e0c045",
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
              "id": "06d24357-08e6-4bfd-9692-20c7380845e9"
            }
          ]
        },
        {
          "id": "cb31b804-c7b9-4a8d-b76f-64f6e7511a7a",
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
              "id": "ab58ae2e-4a6b-4895-8bd7-f1054244bb7b"
            }
          ]
        },
        {
          "id": "95cf82cb-414e-4d97-b0bd-769732f90bca",
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
              "id": "67d1dc7c-a801-4a32-84cf-669c6a9d50a5"
            }
          ]
        },
        {
          "id": "8e0fd128-880b-44ac-8588-7833399e2ee6",
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
              "id": "dc657a2b-99be-490d-ad73-69ab168d168c"
            }
          ]
        }
      ]
    }
  ]
}