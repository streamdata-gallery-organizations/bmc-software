{
  "info": {
    "name": "BMC Software API Get Relay Configuration",
    "_postman_id": "b157c63c-4a73-4ce2-af11-8e1f34e72edb",
    "description": "Retrieves config for a relay host if changed\nIf no timestamp specified, configuration data is always returned\nIf config has not changed the string &#39;not-modified&#39; is returned",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "79e04eb4-6f39-4f07-9d0e-ce20f6e3e205",
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
              "id": "a922bea6-943c-452a-88a6-63b1ef39461d"
            }
          ]
        },
        {
          "id": "d74f49ec-4e38-4718-916b-8ef0bc7cef0c",
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
              "id": "ef70fe21-7c26-4abc-b4be-e08658e67593"
            }
          ]
        },
        {
          "id": "2c14fd57-0623-442c-83ea-9279a722a784",
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
              "id": "955838bb-bef9-4b8c-aaf8-237b650a8bb6"
            }
          ]
        },
        {
          "id": "5bc7b7f7-943b-4259-8387-fbb1cc88368e",
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
              "id": "f90d71c8-24b3-4d94-8c3d-639af2f10766"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "440fb967-aeee-4180-bc3a-eee82657bcca",
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
              "id": "21d2f763-4905-4b3d-81e5-91b11e709fd4"
            }
          ]
        },
        {
          "id": "24296241-2a13-49de-b80c-b1b5b264577e",
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
              "id": "44264fca-fcb0-4d3c-a8cf-510c8f40a63c"
            }
          ]
        },
        {
          "id": "3fd6dbdc-f933-49f9-9b8c-16a7d52c1475",
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
              "id": "ef9f39af-03fd-4bde-baf4-95c06c75b457"
            }
          ]
        },
        {
          "id": "81a2c977-8e64-4390-af4a-5263abfb5f92",
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
              "id": "5e33c26d-6994-46a6-8498-3f34e22a93f9"
            }
          ]
        },
        {
          "id": "f0188366-c98f-4048-b444-23289b331ffa",
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
              "id": "eaf20daa-7b96-4e9c-8b52-87a7c7aed699"
            }
          ]
        },
        {
          "id": "a09cfbf5-4dbd-42e8-b6c7-01f5fa7e877f",
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
              "id": "cd8b0eb7-bd6f-45aa-80c1-2f4ad9a94724"
            }
          ]
        },
        {
          "id": "f2fa5bc0-d367-40f1-8149-ada5cd7d22b1",
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
              "id": "239cb7d7-b761-41a4-ad1d-06930d328f9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "dfea16da-fc72-4189-a9ae-50f41f0678f4",
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
              "id": "778cc5c0-5496-43eb-a3da-ddc5e187606e"
            }
          ]
        },
        {
          "id": "81d36ae1-b7bb-4f65-b2ff-527d6b55243b",
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
              "id": "483f3173-34d0-4fdd-8d72-490e9f3dfc45"
            }
          ]
        },
        {
          "id": "7d917550-b26a-4cb3-a72b-e7221ad70e8f",
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
              "id": "6d4f8f88-f76c-458b-83d5-cacfa5f981ef"
            }
          ]
        },
        {
          "id": "63e7ee31-8924-4ea3-ae60-10e6d006a185",
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
              "id": "33047060-1893-4002-b2ca-7c50f271bf11"
            }
          ]
        },
        {
          "id": "d1f892bd-cce9-433e-bd00-c372a3604780",
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
              "id": "2a3b114d-39cc-4fbe-ac2c-de6babf396cf"
            }
          ]
        },
        {
          "id": "04eeb406-7285-4138-939c-ef378f50f83a",
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
              "id": "dcd13766-e839-4d2b-82eb-3ea3dac56419"
            }
          ]
        },
        {
          "id": "7d8d7d32-448d-4903-9f04-0f5b2aaaa59f",
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
              "id": "e9aa2cc4-9ff2-4132-b297-9324b78bd483"
            }
          ]
        },
        {
          "id": "6887a190-fc91-460c-bdc1-69bab648eadc",
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
              "id": "6abe1fc3-b1cb-4384-8477-092f9ba49282"
            }
          ]
        },
        {
          "id": "7b14bee8-883c-4b3e-b31a-bc3aa33d1fff",
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
              "id": "80974df0-1d55-4a8f-a0c2-44dab12fdc11"
            }
          ]
        },
        {
          "id": "fe6cd5f8-02b0-48b8-8d05-733cb173678c",
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
              "id": "fecc1442-bd5f-4520-8e30-a9816d99eccb"
            }
          ]
        },
        {
          "id": "1f6cf108-aa1d-4983-bc86-68000c63bcec",
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
              "id": "21251c14-3f14-42f0-8f64-7e0d4cf3fd79"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "9d294ec6-a431-4964-b1bb-f8b178b01e4e",
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
              "id": "c27b6a63-5a20-4668-993b-f651ef886cab"
            }
          ]
        },
        {
          "id": "80f61499-0bf9-44ca-9b77-b757ee8dc2df",
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
              "id": "61bf9cac-2a17-4fa0-ae62-9a5112835b1b"
            }
          ]
        },
        {
          "id": "04d6d021-b8b5-480a-9ad1-fefc47aac3d1",
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
              "id": "35e49944-539c-49d6-88e3-64533f3c2764"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "3bc97e66-bda9-4949-b033-2032a492b754",
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
              "id": "3b9c2710-99f0-400c-bcee-dae538b28a32"
            }
          ]
        },
        {
          "id": "9401cbe3-b98a-4dc4-b96d-c5a812457797",
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
              "id": "bc31636b-4382-4ac2-8d67-f74238849f5b"
            }
          ]
        },
        {
          "id": "67bf5f99-4c12-4535-bd05-b7d782dba4a9",
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
              "id": "0e027c1b-e855-442d-ab18-f869f0546bea"
            }
          ]
        },
        {
          "id": "ffcd683a-520c-4798-a7aa-08003a4e59f7",
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
              "id": "27f617ba-32ff-40e0-acb3-8e2e1673af8d"
            }
          ]
        },
        {
          "id": "e8b11110-1628-469d-b23d-8f27e96a135b",
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
              "id": "981affa2-a4d1-43c4-86c5-cfa2159db03a"
            }
          ]
        },
        {
          "id": "58bbe8bb-d0f0-4874-90b6-0d3398d92253",
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
              "id": "c1a94120-9860-4944-aed2-ec93127572e6"
            }
          ]
        },
        {
          "id": "d23dd22a-1997-42ed-b262-f8f84e55d24b",
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
              "id": "6cf82ea2-90c8-4120-a27a-6d2b1e99c732"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "7a7f3591-3237-4c88-b619-205cf88300ac",
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
              "id": "eb1cb3cf-ab29-4a11-98f8-f504fc4cfe4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "d020ce1f-3e3e-4d86-a87a-dfadecfd7bad",
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
              "id": "c6fd7288-d28b-4181-947a-012960f0c06b"
            }
          ]
        },
        {
          "id": "b2a2fa32-244a-4dde-932f-5eaf983f50a5",
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
              "id": "477a4a8c-ef58-4b6d-b261-f3f1914a7841"
            }
          ]
        },
        {
          "id": "700776d4-5789-4f6a-8b1f-09246f223b0d",
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
              "id": "b9e58e1f-b940-41dd-89a9-bc139ae7ad07"
            }
          ]
        },
        {
          "id": "8de7092f-11a0-49eb-83c5-d165e9d6de4a",
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
              "id": "5af70282-377d-4e24-9078-36f0bec2175f"
            }
          ]
        },
        {
          "id": "946b2052-6b79-4973-8f26-fd0090cf256b",
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
              "id": "729f2813-8cd1-4f76-a686-84a69e0011f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "69622d7a-fd35-4cfa-99ea-01cabcf62f95",
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
              "id": "67e4ecd4-5ed0-47a7-9e4a-23306f899131"
            }
          ]
        },
        {
          "id": "6edca391-2ea3-4982-b38a-68b8c00da5af",
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
              "id": "440c4e64-770c-415b-815d-72ada5643839"
            }
          ]
        },
        {
          "id": "c8489a56-bbfb-4d48-8d6f-063fe4d20e35",
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
              "id": "8f7cae7c-a18a-4e77-9aef-c1ec8d3f69f0"
            }
          ]
        },
        {
          "id": "e23253f1-2902-4524-aef3-580f421bdc65",
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
              "id": "530e5289-a1ad-45ef-af5c-acb5394650b6"
            }
          ]
        },
        {
          "id": "4b51f038-2f55-4da6-a719-e39cec7a7218",
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
              "id": "76df6de4-6231-4470-9aef-5bc0bf1ea3a1"
            }
          ]
        },
        {
          "id": "5d014f7d-3e60-4980-b364-132ed5da305d",
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
              "id": "223a2ced-58a2-41b8-833d-5b88a80948fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "e7c3b7bd-fd27-4f6e-8e10-07004c06b277",
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
              "id": "a34ba4a3-6976-4b41-ba03-a577bd4b99ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "62a209b3-4055-402a-8222-5377a33714dd",
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
              "id": "67076954-b95a-4bce-a770-0560327d6076"
            }
          ]
        },
        {
          "id": "165614ce-3027-4629-b059-a7c5d35f5d69",
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
              "id": "6cdee280-ae92-46db-bdd5-aba91536e8ca"
            }
          ]
        },
        {
          "id": "bf37ead8-8479-46bb-aea7-b1397fe592bd",
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
              "id": "f1d62360-f54a-46a0-bc2a-be7ee6354478"
            }
          ]
        }
      ]
    },
    {
      "name": "Plugins",
      "item": [
        {
          "id": "5f960052-5fb3-41eb-a356-2f84474e02c4",
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
              "id": "9cf90fa2-cf0a-4b68-a704-ee51b0f9fe69"
            }
          ]
        },
        {
          "id": "f48cadca-1a26-426f-b79f-c57c09424dee",
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
              "id": "9918e0ba-8e86-4863-9181-e04e793ec360"
            }
          ]
        },
        {
          "id": "eac82fbb-82cf-4765-9a84-e3ed7e2ddde0",
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
              "id": "3c65d46a-a218-4151-899d-9feb67c38d27"
            }
          ]
        },
        {
          "id": "ac2bcf95-a39d-4b55-a74c-41589d363b38",
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
              "id": "bbc43738-5dc5-427c-b986-97024ac95766"
            }
          ]
        },
        {
          "id": "19593f77-283a-49f3-aac9-9c2e4fa22546",
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
              "id": "1eeabb9c-802e-4606-b3e2-945b86d2d16e"
            }
          ]
        },
        {
          "id": "5a7e664a-ce58-4876-9166-d7ab55a5ffa8",
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
              "id": "d3145f5e-2635-4b8e-9092-274f68f28c26"
            }
          ]
        },
        {
          "id": "2455ebeb-757f-40e6-a506-c135aae829af",
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
              "id": "c5f55ec1-f99a-4f48-a847-0e11d545140b"
            }
          ]
        },
        {
          "id": "ed1655d6-f907-4010-ba10-ea3554844aad",
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
              "id": "f93e23ba-f350-4ef9-a55e-bc46b48ea44a"
            }
          ]
        }
      ]
    },
    {
      "name": "Relays",
      "item": [
        {
          "id": "93d42247-3cb1-4abd-9248-763a0f55aa46",
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
              "id": "d6c1bcde-0043-465b-928a-6e6d6cc7eb69"
            }
          ]
        },
        {
          "id": "d5300161-a447-4a07-8ada-2521eeade367",
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
              "id": "4bc8e625-50da-4a99-b18a-f524c5afd303"
            }
          ]
        },
        {
          "id": "b0229c6c-bb93-4a0e-854b-fade1fa2f95d",
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
              "id": "23a86a42-a0a3-4b9a-9a17-e5e3937833a4"
            }
          ]
        }
      ]
    }
  ]
}