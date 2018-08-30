{
  "info": {
    "name": "BMC Software API Get list of active metrics",
    "_postman_id": "095eb9e9-bfc5-4703-a263-9d15a7edb19d",
    "description": "Get the list of actively reporting metrics from a given time until now. This endpoint is not available in the Python and Ruby libraries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "ed7a6afb-0fdc-4869-8485-c0ec195e64f5",
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
              "id": "b9318531-2054-4aa1-98c6-fa02eba21f44"
            }
          ]
        },
        {
          "id": "f72f24f6-a024-4fc6-b688-560445e57992",
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
              "id": "f0589f0e-6570-424e-8662-3b5e22aae22a"
            }
          ]
        },
        {
          "id": "3c5a9560-82f2-486b-a831-1a4849ce3523",
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
              "id": "a4f2c606-3399-45b6-9af4-a743b445bb39"
            }
          ]
        },
        {
          "id": "299a51db-e9e4-4dff-8f69-a28aaf5de2cb",
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
              "id": "135b771c-5953-4d97-a751-8e741ee611d2"
            }
          ]
        },
        {
          "id": "783852fd-2f14-4612-9c30-5d5ed7a49111",
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
              "id": "be2ac824-a5de-454f-9c65-94049da422c1"
            }
          ]
        },
        {
          "id": "91ec1f04-8fb7-4933-937a-101443bc4bd7",
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
              "id": "1ab60d2d-2687-4d4c-8591-d237490b4b77"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "cd3fec33-2b62-4d44-b47d-f2a18bd07598",
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
              "id": "eab897c6-7f3a-49ad-9106-6b58654ad3c8"
            }
          ]
        },
        {
          "id": "7a927bd8-e1d1-43f9-b85b-825befa78d42",
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
              "id": "d3354b71-87a7-4617-a8c7-7aca05b97136"
            }
          ]
        },
        {
          "id": "d338a287-5f1d-46d2-8d2b-a0f38d8f9c64",
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
              "id": "9d115a9e-a1ca-47ba-834c-6215adf49dc0"
            }
          ]
        },
        {
          "id": "85aff362-f4ca-4c01-b3ee-be4765603aeb",
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
              "id": "be95f28b-5ef8-4a3f-b0f4-c0e553b390b7"
            }
          ]
        },
        {
          "id": "1fa024a8-47f8-4919-b707-65146a45c3ef",
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
              "id": "abad7b4b-d171-4fde-81e1-f1c83a4a180f"
            }
          ]
        },
        {
          "id": "4ac675ff-5c72-4ca2-be8e-0140955ea871",
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
              "id": "e8197b17-7bb1-4978-adeb-050520fd6c35"
            }
          ]
        },
        {
          "id": "1de1a9ac-561c-47bb-8bf6-ae608572495e",
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
              "id": "dedbd9f1-ac76-4134-8288-ff1030617e1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "69ec4235-aeb2-4957-9f91-dbadbf5048a0",
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
              "id": "51afb455-a249-4838-b703-d122297db9e4"
            }
          ]
        },
        {
          "id": "5934834f-9768-4235-a557-6a03abfe144b",
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
              "id": "b43af4ae-7923-47d1-83c4-5988ee1c1a36"
            }
          ]
        },
        {
          "id": "99907731-41ab-44cc-ac60-0e529414f5a1",
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
              "id": "d3ad7d8d-6e01-4c99-911f-23ebabf5a1b0"
            }
          ]
        },
        {
          "id": "162ddbb4-8167-4268-83da-544746ec5a29",
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
              "id": "9f0bbb4f-4df5-41ed-98fa-6f83ca70864c"
            }
          ]
        },
        {
          "id": "50e6b88a-ffbc-4dea-82ca-c7aff5870715",
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
              "id": "48e513f4-b9ce-4b9a-bcf6-869ffeb28825"
            }
          ]
        },
        {
          "id": "00e9dadf-6e4f-4460-a7f3-2252c6cb085d",
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
              "id": "e30ba02a-1d16-4002-a5a5-3997efc18fa9"
            }
          ]
        },
        {
          "id": "2974aea6-5a9b-46fa-9ad6-6eb63399a6d2",
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
              "id": "a82d4ec5-03b6-42d7-834c-1cd663a8d328"
            }
          ]
        },
        {
          "id": "17bfb3e0-3b80-4165-9295-c8bc0f263673",
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
              "id": "5606f976-44a1-4b71-83a0-956c3dcf529d"
            }
          ]
        },
        {
          "id": "73fe7988-3eda-49d9-a04e-a45309a16779",
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
              "id": "f5f3ec93-7785-4608-a3d4-20572173dac1"
            }
          ]
        },
        {
          "id": "dfd2c8fd-378b-4689-b2a9-a22c06ca6b26",
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
              "id": "f2dc5ac6-6032-40be-8e8e-a5b7c0db459f"
            }
          ]
        },
        {
          "id": "a69ee1aa-bfdd-41a8-aee3-d537f46c67ab",
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
              "id": "0d0e7f5d-88cd-42ad-be4c-ec01f1c353b7"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "5cf47439-22e4-4aae-bdfe-4cd729356cb6",
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
              "id": "07c25017-4467-4303-ae58-b5a6aec03d92"
            }
          ]
        },
        {
          "id": "622f09cc-7680-474e-8429-f1c83c704dfa",
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
              "id": "184b644d-058d-41e7-907a-b42c996a3340"
            }
          ]
        },
        {
          "id": "3d9de27d-a47c-40c0-941b-a22d2cd0e651",
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
              "id": "e45d67f8-4b60-4be3-a35f-0d3e1bff81ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "3fc7e167-d9e3-489b-aa6f-440977f32a23",
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
              "id": "68fe2cc0-659e-4d2e-a772-8f03a15df13e"
            }
          ]
        },
        {
          "id": "a9b185d8-b870-41e7-9562-355b3a6aa175",
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
              "id": "6a85f1a7-623e-4afc-b4f6-7f085f51866b"
            }
          ]
        },
        {
          "id": "28536c7e-c07c-42a3-b106-040b6e098d72",
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
              "id": "64316343-34d6-4444-a936-731026dddfce"
            }
          ]
        },
        {
          "id": "3282881e-21bd-40ec-8fac-1abd7f484406",
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
              "id": "317c1bbe-c18c-426a-8454-3c19bf52f6fb"
            }
          ]
        },
        {
          "id": "077b5e09-5469-4cdb-a41e-47cff0f29d84",
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
              "id": "46307dc4-4c62-4838-a030-2275e83d6096"
            }
          ]
        },
        {
          "id": "e93b49ed-13da-48ba-90a2-f41480647655",
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
              "id": "f73ec6f2-3987-45c6-8373-30c71bccc63e"
            }
          ]
        },
        {
          "id": "edc6c200-5a50-4e5a-bc05-e31c721eda73",
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
              "id": "5bf4a3c6-d1bc-4fc2-bbeb-4d35829bb32b"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "d3381d30-6fac-4bda-92c5-f2139e05bbe7",
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
              "id": "146b554c-a90f-4cf9-ac18-0b419db81c9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "d4b973bb-4a6d-48ee-9e9b-37d84493005d",
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
              "id": "9fa34961-8e4e-4df4-92c0-0103005f18b7"
            }
          ]
        },
        {
          "id": "0291b9d1-e537-4463-8526-acd6a7e6de07",
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
              "id": "59cf99ce-49d1-40f4-b33d-6dfa2aeff932"
            }
          ]
        },
        {
          "id": "8918761d-476d-4ecf-8e96-5119d6162e22",
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
              "id": "d8980136-1b71-4582-ade7-7be6b2faa115"
            }
          ]
        },
        {
          "id": "3dbbe36a-605d-4f2f-a7ae-7a7992190d13",
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
              "id": "7de510e3-ac03-4142-baec-4d7ad3ecc16a"
            }
          ]
        },
        {
          "id": "015e1e5c-6e5a-465a-98e8-44b757d6c3a5",
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
              "id": "9c3fef29-9a33-40ff-a791-cd0d4e6d7b29"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "6a4c34b2-4026-46ca-b92d-cc9fd6b11a9e",
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
              "id": "db8c399a-35cf-44a2-ada2-a446e3060650"
            }
          ]
        },
        {
          "id": "c44a9a6f-7f82-484d-ab24-7db1d2c2af1f",
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
              "id": "32fa1458-bccb-47cb-b063-37cfbeda38bd"
            }
          ]
        },
        {
          "id": "d46b3fc5-e4bb-4932-9eee-49b2bc017e91",
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
              "id": "e9ce2fdb-4649-4559-909e-7025acf5a89f"
            }
          ]
        },
        {
          "id": "fa484c9b-8a28-4fbf-a451-6f962cdab61c",
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
              "id": "5758fa80-32a9-4d33-8fbb-224f06213ffc"
            }
          ]
        },
        {
          "id": "0076e289-b1da-4d4c-a565-3e8e9725c677",
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
              "id": "91d2b46c-6aae-445b-a2b5-9b269c8792a4"
            }
          ]
        },
        {
          "id": "322a402f-0663-44cd-bdc8-ac65194a20a6",
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
              "id": "590966a5-4b3a-4189-b8dd-968bf0af2c2d"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "b1f935e7-be07-4bc7-8fdc-60b19d71ba94",
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
              "id": "07e5c8f9-9087-4a37-8822-0333942206a9"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "89159b89-d764-469f-af9c-abb7d8122605",
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
              "id": "2d081e60-bf71-4de8-ab48-79ee022fdac6"
            }
          ]
        },
        {
          "id": "25be0414-dbe2-4a34-9825-3d353694d36a",
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
              "id": "d99495a4-0336-4e25-9f9a-8509a2585df4"
            }
          ]
        },
        {
          "id": "a7d11ca6-3b84-435e-8e20-9eae26669d06",
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
              "id": "c0be4f78-3d4e-4ab8-82e2-f6fbc79d2ce2"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "a53a6033-608e-4c19-849e-54b7c1ef591c",
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
              "id": "a5877cf9-9a84-48ac-bba5-1b4495a1b0be"
            }
          ]
        },
        {
          "id": "340618b6-605f-4c27-b1e2-38250f5966d6",
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
              "id": "b5edc27c-f823-4771-b25e-1a8ee73ddea3"
            }
          ]
        },
        {
          "id": "ce6ad659-c4bd-4c94-8b82-3c52bce5add1",
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
              "id": "93f553ae-11c1-4da1-9bec-dbe5b5d84cf1"
            }
          ]
        },
        {
          "id": "62bc2af6-434c-4b0b-8505-175df9f1937c",
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
              "id": "9b43b81a-10cf-4ccd-ba90-4992732bd652"
            }
          ]
        },
        {
          "id": "4b5a28b5-2d03-4655-bfd2-844c9be953fa",
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
              "id": "95340459-95fc-4549-8228-8f7f95259bc6"
            }
          ]
        },
        {
          "id": "952df0b7-b9f4-46ee-a421-2b89d2d267fe",
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
              "id": "2cfacee4-749a-415c-aeef-ee3ac67a9fb2"
            }
          ]
        },
        {
          "id": "cbd58edc-7904-45bb-8ddd-107fbd451a52",
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
              "id": "26d445ff-2c9c-4cba-aa47-f7ad82de25fb"
            }
          ]
        },
        {
          "id": "36cfd752-4b42-4038-ba76-f065ad61e29c",
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
              "id": "e046272c-8b77-40f2-b09d-a6f7b89e6f2e"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "bee0e62a-263e-4a36-8cb4-9b37e8edeb54",
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
              "id": "45cf7866-0071-49d7-8a8d-5bbb8848a6b6"
            }
          ]
        },
        {
          "id": "393544a6-924b-40e2-81c2-6ed799bcedd8",
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
              "id": "c7df0fd8-544e-4f56-9bcd-e3b638caa1ca"
            }
          ]
        },
        {
          "id": "04e38a00-7964-45fb-bd62-d9068bf3ca00",
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
              "id": "eec1920b-1fc0-4b7d-9fa2-e40f23b34627"
            }
          ]
        },
        {
          "id": "f129facc-6913-4516-bb7a-7a4686ca32d5",
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
              "id": "6236d4ea-f955-4936-af94-2fdb5ec6dc36"
            }
          ]
        },
        {
          "id": "483475dc-0435-48c8-a2e3-9d2c1bfaa708",
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
              "id": "5f663551-bf3f-4fee-b242-3f0955dba513"
            }
          ]
        },
        {
          "id": "93269a4b-247b-4e1e-94a0-e5ed6b6c09c1",
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
              "id": "b21da1ed-61a5-4798-9424-75bdce9ff0b0"
            }
          ]
        },
        {
          "id": "cbe96d89-ccbd-43b1-977c-801502548133",
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
              "id": "e87240b9-08fd-4f2a-95f1-ade1b28d7fc3"
            }
          ]
        },
        {
          "id": "6d6e3148-768e-41d4-a3f8-7c4fa6007052",
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
              "id": "4ee89bcb-0c38-4e88-b8dd-65a8a3910d67"
            }
          ]
        },
        {
          "id": "be236a8b-8cce-4d93-9982-54f452d24aab",
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
              "id": "a566f968-72c0-4e61-b0ed-23cf8ce1f1af"
            }
          ]
        }
      ]
    },
    {
      "name": "Sources",
      "item": [
        {
          "id": "21d82fc9-f7fa-48c7-9234-cfc938832193",
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
              "id": "b3ae545c-d405-4d1c-a664-663acc580ff4"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "ad7107bb-be11-418b-a2ee-fea6e6cd6a0e",
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
              "id": "e7b470d8-d655-4b23-8dfd-235323c9f2e6"
            }
          ]
        }
      ]
    }
  ]
}