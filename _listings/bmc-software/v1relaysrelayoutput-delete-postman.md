{
  "info": {
    "name": "BMC Software API Clear relay output",
    "_postman_id": "6f8e14f2-27cc-452e-a8ee-47f3311004d2",
    "description": "Wipes the logged output from the relay up to present.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "845c2f29-4359-4b40-8438-c6e9113457c6",
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
              "id": "a6991c7f-8ce9-4035-b0e7-b695c6faf81a"
            }
          ]
        },
        {
          "id": "441fad2b-4d4c-45c3-b4b6-5f87ff3e1454",
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
              "id": "6bc5ac84-c40b-4b3b-bfa5-393061ee6cf2"
            }
          ]
        },
        {
          "id": "82c94b20-30b6-4bc8-be70-a56e22254e16",
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
              "id": "b8ab9bda-2ecf-4932-ad97-d1ee362f4142"
            }
          ]
        },
        {
          "id": "98dfec8d-1a75-4da6-9934-c856e9092433",
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
              "id": "6c71f490-198d-4f18-a149-a9c486a791d8"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "896c655c-d140-4a37-ad5f-b97b498accd0",
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
              "id": "ab19b292-6615-4536-9658-231bf42ddb60"
            }
          ]
        },
        {
          "id": "a90b7e2f-f211-4d3c-b06d-e70c0a72921b",
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
              "id": "4fba93b9-f6f1-4bb6-ae03-d70defa6150f"
            }
          ]
        },
        {
          "id": "7dc3c0b9-6252-4410-a43f-dd067e67e272",
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
              "id": "d6cf87e3-499c-4f45-bd06-b432eb64637b"
            }
          ]
        },
        {
          "id": "7e2a4220-977b-4033-85e0-c58e84fedd9f",
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
              "id": "cceeec69-2210-4349-b4e3-acb08f1928b9"
            }
          ]
        },
        {
          "id": "86fc6429-4667-441b-8dca-6b47eda1e568",
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
              "id": "23b70f2e-f796-4d1a-a447-e571f4fe0db5"
            }
          ]
        },
        {
          "id": "d19242cf-4f6b-43b6-9dbb-355422d04705",
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
              "id": "f2d77558-7767-4519-b342-e735033566b4"
            }
          ]
        },
        {
          "id": "ef8a177c-88d3-4822-870e-6650f87aa01d",
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
              "id": "187784d9-9297-40b7-9b7c-ed145ccf3266"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "b42e73ce-8bc4-43a7-a03c-3b8c0c1d184d",
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
              "id": "dcd8b71c-8cce-4447-aa01-d87ebe126c41"
            }
          ]
        },
        {
          "id": "c4847e1b-4a4f-4e21-8865-9efb8be73865",
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
              "id": "331d85ad-304c-4ed1-8e97-824c59e9411e"
            }
          ]
        },
        {
          "id": "9877c48a-3ccb-4c88-8e6c-a75e7677345f",
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
              "id": "793664bd-39be-4a40-8b4e-04f0dd02115e"
            }
          ]
        },
        {
          "id": "553fac9c-bb82-4c38-ba08-ee5ac7ee403b",
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
              "id": "f43fdf64-ef95-4072-ab26-b190bcead06e"
            }
          ]
        },
        {
          "id": "fc1bf0c0-a140-40a9-b54c-5b2ac8c51132",
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
              "id": "c1662acc-c0d3-415d-bfff-023c9494103c"
            }
          ]
        },
        {
          "id": "0dbab177-9f16-4d41-a639-e0c0f05c29f3",
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
              "id": "bfb461d8-5b82-4ff3-85d3-473ce7f1d5cb"
            }
          ]
        },
        {
          "id": "4ac5d8f7-87d4-4183-bb26-65230500733f",
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
              "id": "ce167592-17f7-4d00-a540-6304ab497412"
            }
          ]
        },
        {
          "id": "45f4244b-2222-4320-96ad-38eb9d9a42bb",
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
              "id": "504fcfe5-d524-4a4c-9a57-e24deb0a7887"
            }
          ]
        },
        {
          "id": "914b2c0f-a2b9-41db-8894-ec9bd9b9537f",
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
              "id": "a19ff089-07c6-4779-aa49-cc2dc2994115"
            }
          ]
        },
        {
          "id": "7639b9b4-f4d9-416b-85ad-31801d0fb0bd",
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
              "id": "77f20db2-aaed-4c00-9873-a0327d75d5ee"
            }
          ]
        },
        {
          "id": "b52bc88c-64f6-4ae9-949a-8a57399c36eb",
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
              "id": "b78d2677-9a35-4256-8e6b-78de9ed86c98"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "9f659edd-852a-4631-b27b-03fa316926a2",
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
              "id": "10daaf77-6b67-4c2a-b0b1-0ddc3536fc33"
            }
          ]
        },
        {
          "id": "ba69f588-30fc-4f33-941a-778d3b94ad10",
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
              "id": "1b633a01-8331-4381-8ae2-a95e462a02f4"
            }
          ]
        },
        {
          "id": "c52d9b32-77df-47d6-a767-febcc27975cd",
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
              "id": "0755ea9a-d254-4b64-86fd-65ca159b4845"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "4d909edd-02b5-4e56-8e31-96de06a12a30",
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
              "id": "7f42f6ae-e50b-4483-963a-fc9e1c87345b"
            }
          ]
        },
        {
          "id": "139f4d87-e2f2-4bf9-a8a6-19bda427f6b4",
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
              "id": "45e0bb38-73f9-4039-a956-18dede32fb0d"
            }
          ]
        },
        {
          "id": "ac508797-ee23-41a1-815a-ddee73f510f5",
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
              "id": "a82c9897-ca4e-40aa-bdbc-eda355aed07e"
            }
          ]
        },
        {
          "id": "ee6b5459-b1e8-4e98-a665-9db47b8795bb",
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
              "id": "0baf0a6e-0e30-458c-85ce-72417cf587cb"
            }
          ]
        },
        {
          "id": "33e7a5de-f094-4c62-a690-b21578d014ab",
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
              "id": "6a1bf6d3-4b38-44bc-b3fd-0780e752210e"
            }
          ]
        },
        {
          "id": "34e357c6-14c9-41b2-b50b-6e1d20fed10c",
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
              "id": "0e53b5be-2bcd-49e0-8496-acc949c4cdf8"
            }
          ]
        },
        {
          "id": "c9c9f80e-8bb2-41ec-8ac6-67ca4cb226bf",
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
              "id": "de60523f-c2f1-493f-82ef-beb3b7955461"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "9265985b-ed15-4303-8a2d-90bf4bd545af",
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
              "id": "5896aa89-e55a-4422-b79a-ee6e8a0de539"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "ba004723-9f85-435c-8fb2-cf17fe686ea9",
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
              "id": "5ed8022f-5dc4-4c33-9975-fb38fb066fbb"
            }
          ]
        },
        {
          "id": "1230c5a5-9a3a-4f23-bde6-5783aa7eb421",
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
              "id": "31c26fb7-36e9-4825-bb48-2b0e2dedbc31"
            }
          ]
        },
        {
          "id": "fbc4913b-8b03-4859-bc18-740ef8e186dd",
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
              "id": "a2dd2ed7-c8ec-4835-966a-28425ea8483f"
            }
          ]
        },
        {
          "id": "e7b49694-1d9a-4d88-b72d-2f355ab6ab73",
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
              "id": "2b8e513e-2022-410d-b0bb-ed3def186356"
            }
          ]
        },
        {
          "id": "d0e60b06-cc8f-43de-8cfc-f4e7364c8981",
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
              "id": "95b66183-2afb-4655-a8bb-55c422e6db8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "e284653b-b512-4860-b796-5a143108443f",
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
              "id": "39ea3e4c-2b87-4520-becb-dad221fcc622"
            }
          ]
        },
        {
          "id": "bdd41c6a-a056-4200-8fe9-96b9753167c8",
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
              "id": "c5f462f2-d4aa-464e-8f54-8f6a0f5ae6c0"
            }
          ]
        },
        {
          "id": "956e3819-0bf1-4260-a8a8-d65f3d47e0a4",
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
              "id": "db7f60f7-541c-4d79-bd7f-c7f2dcba3b46"
            }
          ]
        },
        {
          "id": "ece44b8b-d548-4348-bd03-2201ce316f8b",
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
              "id": "f94479e0-a87b-40b4-a668-286ffa309df9"
            }
          ]
        },
        {
          "id": "c90fe991-01d9-400e-a236-3807b27b9ac0",
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
              "id": "06872f52-b1de-4fd8-b0b7-793d1225a8da"
            }
          ]
        },
        {
          "id": "eb574164-3fcc-4f5e-8b25-c554f6694163",
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
              "id": "1ffd17b8-0135-4683-a270-5814e42edf50"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "67e8ca64-348b-49e5-a69e-4f0f8e0368c4",
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
              "id": "c0076ea3-8d64-44e9-9fe3-1cde9822cb6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "6fadc726-b5f7-48c4-91e3-dd0f7c5d0065",
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
              "id": "8c65d42a-af66-4e80-8883-54f231f5c2cc"
            }
          ]
        },
        {
          "id": "3199abaf-3704-45d5-8175-43e358855572",
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
              "id": "5a04fbec-b028-4e43-971b-ae625aef17a6"
            }
          ]
        },
        {
          "id": "7d59433f-dfc5-4fd5-8e20-2d610e4ce7f4",
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
              "id": "50d9712b-1811-434d-b54d-32e6bad77822"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "48793546-4236-489a-a7b9-5d9dab6a2ace",
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
              "id": "e1a4da90-4efa-496f-9076-11fcc2d9e4ab"
            }
          ]
        },
        {
          "id": "e156a1f6-c8e2-4b39-bdb2-ad54cd460add",
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
              "id": "7f0106fe-7989-4216-bf96-4365a6b449f9"
            }
          ]
        },
        {
          "id": "0e7e34c1-cab6-4276-a86d-4510823264cf",
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
              "id": "d4bb2060-e859-4cac-a682-ccfbeb7b0f8f"
            }
          ]
        },
        {
          "id": "e51fdbb2-b5f4-4414-a70e-8e4f1d8fba7c",
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
              "id": "bdefc5e6-480e-4783-b8cc-82df0a6ceb30"
            }
          ]
        },
        {
          "id": "a8f08052-137e-4271-88cf-eb38f7b23496",
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
              "id": "35107f1d-7179-43b2-b649-a3b833716fad"
            }
          ]
        },
        {
          "id": "8ccaab04-7518-43ef-9225-47ce6c460d90",
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
              "id": "59e0eed3-e8d6-4aa0-8374-992521c196ee"
            }
          ]
        },
        {
          "id": "e4ce3e46-b99f-4b25-9d53-c596eddc2d68",
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
              "id": "39a87d46-5f8b-40de-a330-51b95c326d3f"
            }
          ]
        },
        {
          "id": "a574ac0c-9bbd-4487-b120-fc236d309ce0",
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
              "id": "dcc7233d-1c34-4536-8d0b-34acd25cd7a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "427c5ae7-a165-4545-8322-c90723ef18da",
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
              "id": "4148fddf-aaf5-43d1-aaa4-8ef69afa5d1e"
            }
          ]
        },
        {
          "id": "4b5676e5-f74d-4bf7-b747-4a623d6afe50",
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
              "id": "98e64480-6da4-431d-8e23-a38530fa122c"
            }
          ]
        },
        {
          "id": "4b8f717a-d949-4f5b-b938-4156ce03049d",
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
              "id": "11e4d429-958e-4072-8197-40cf0e47ce6b"
            }
          ]
        },
        {
          "id": "d6941207-d255-4a5c-96b1-b9e82516c50c",
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
              "id": "32909328-fd68-483c-a571-10a70535498d"
            }
          ]
        },
        {
          "id": "07790dcc-4e15-4398-be6a-4a5581d1a023",
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
              "id": "be5afedc-d2cd-43f7-8a2f-8d08b66049f3"
            }
          ]
        },
        {
          "id": "05ba1e7f-11bd-47ae-8300-341cef63c820",
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
              "id": "fd07531a-158e-4b8a-988b-c39f919adb38"
            }
          ]
        },
        {
          "id": "46dcad68-19b3-445d-8f78-0437c9617251",
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
              "id": "ac71c132-e230-4de2-85aa-dfc7c4ac53ec"
            }
          ]
        },
        {
          "id": "8efbb16b-4fbf-4794-9672-0e42ad6cb181",
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
              "id": "c7934303-8b08-4ae4-8e1c-ead77951bb2a"
            }
          ]
        },
        {
          "id": "99a5be3c-28c8-4b41-b082-3b23b1d9522f",
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
              "id": "6d874618-f65d-4a97-a556-6dba3d3f7ae7"
            }
          ]
        }
      ]
    }
  ]
}