{
  "info": {
    "name": "BMC Software API Get measures",
    "_postman_id": "a88b02b6-a13b-4be6-a2eb-d408f48ce690",
    "description": "Retrieves measurement readings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "ffd1e056-976e-431c-816d-895e573d9e2c",
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
              "id": "8b8f7186-579a-4de7-be09-28821fba698b"
            }
          ]
        },
        {
          "id": "333014ea-ce2d-4387-b8cb-eccc775082e3",
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
              "id": "400d6ffd-a665-499b-9a8b-253c4e58aa57"
            }
          ]
        },
        {
          "id": "269b0eca-ddc3-45bf-9407-f83c6237b9e7",
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
              "id": "03b3c1b8-25bc-462d-8c79-dcdf03ec3aff"
            }
          ]
        },
        {
          "id": "88c754d7-8733-4e3f-ad0e-305d50f13b7b",
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
              "id": "36e9168c-8ef6-472a-95b1-a4085c57b4e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "7531f9e6-820a-479e-af5d-c5252b1e087f",
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
              "id": "88ed0fca-337d-48b6-838e-5e2c337600fa"
            }
          ]
        },
        {
          "id": "959d4879-b50d-4f4d-a7c5-8fe4abf996f4",
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
              "id": "2f1275aa-5359-4c65-8d1a-79a4e9c10748"
            }
          ]
        },
        {
          "id": "44cb69f9-a0d3-4965-85dd-fb3e99972cec",
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
              "id": "55f8e709-1c7b-41c1-8e4a-4f108e49a751"
            }
          ]
        },
        {
          "id": "b11a09f4-646a-49e4-a5a5-91b00fdec399",
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
              "id": "8c2bddae-a523-4725-8260-da750178d0f5"
            }
          ]
        },
        {
          "id": "f86d6fa7-c15c-4691-9d56-d0b173f0f281",
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
              "id": "fae21a5d-53f5-4bb5-8bfd-6298c1ebdc48"
            }
          ]
        },
        {
          "id": "8e1966d6-ec61-4db5-8c9f-3280212d730e",
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
              "id": "3db50e61-5346-4afa-9858-8e433dad3cd4"
            }
          ]
        },
        {
          "id": "87147e44-4ed7-4c67-becc-f44ea66c0148",
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
              "id": "782ef49c-5194-4634-b633-fbf0f5e7240c"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "7f244a77-dabb-4f4d-9951-4271aaeb9078",
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
              "id": "afc7e64d-1aeb-44a1-a3ff-ff03cd2ee756"
            }
          ]
        },
        {
          "id": "ed81d19d-c923-4b3b-af98-c1f7b8cc8225",
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
              "id": "e7a13e81-1ba0-451a-a72c-18e7a15a1761"
            }
          ]
        },
        {
          "id": "a8f7d196-8d5c-4116-ba9d-821794b105d5",
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
              "id": "b32948ae-5a3d-4137-a4a4-2c68a555633b"
            }
          ]
        },
        {
          "id": "57448208-ca60-422d-90d5-335b030fa11d",
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
              "id": "58e102f7-a2db-473f-b027-2d006de1ac5b"
            }
          ]
        },
        {
          "id": "dde40352-9c24-4b14-9b2f-b89507b119e2",
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
              "id": "27c5129f-a003-41c4-9a7c-bf262ab5cac8"
            }
          ]
        },
        {
          "id": "29f183e9-d6ae-4057-8af7-dd42d6764b0d",
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
              "id": "e86fc002-8d7f-4607-9b4e-5dfc610c2129"
            }
          ]
        },
        {
          "id": "0dfa3fe0-ba8c-42de-b498-f5d3b7b342d2",
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
              "id": "59aaa247-36ac-4536-8ecf-94f0cee98159"
            }
          ]
        },
        {
          "id": "10df1d54-fb30-4922-afeb-fb8793b4c500",
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
              "id": "db89de20-c5e7-4b09-a894-1951063dda02"
            }
          ]
        },
        {
          "id": "a0b2a4b1-6393-417b-b304-7c5f79c6cf6c",
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
              "id": "0716099f-4462-41f6-9a47-ab35bb5ad144"
            }
          ]
        },
        {
          "id": "6e21c94d-8717-4f55-b348-432503f21845",
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
              "id": "1175ce94-2a55-469f-907b-005d83d5f646"
            }
          ]
        },
        {
          "id": "14af358b-a486-4b08-beb1-e792cc54b317",
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
              "id": "6c693589-5207-4e87-be4b-e811148515ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "c2bf94b3-4e10-4a06-adf0-c9bce7746313",
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
              "id": "ef3d372c-11f0-4c37-b96e-568cd2c703f1"
            }
          ]
        },
        {
          "id": "02a09357-63f2-4af4-ba28-4c8267ed959b",
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
              "id": "a663b0df-1c8d-4514-8970-ce00a38a8a18"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "6251a944-ba67-4ce3-bec8-468cadefeed4",
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
              "id": "f943f128-2773-402a-92be-cfb91d71db12"
            }
          ]
        },
        {
          "id": "20151f2f-5e94-452a-a765-538f84009e09",
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
              "id": "ad59db1b-60d8-4b21-956d-8532836712f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "a9f33e37-c0a3-4bc8-a963-f260731f1b69",
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
              "id": "a08f1394-9c31-4568-9184-e245485f2cbe"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "01cd52c6-aab2-4827-8207-095e381fcd03",
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
              "id": "eb812e88-aac9-4f3e-93ac-bb8ec7f89f01"
            }
          ]
        },
        {
          "id": "828e8cf5-229c-467e-9dfa-da4e78c5ea72",
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
              "id": "6b51d896-6ed8-40cf-8846-861a0a94da4e"
            }
          ]
        },
        {
          "id": "698914da-7d59-4329-9037-3a703afdb702",
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
              "id": "81ca40db-da9a-403c-8dbd-9d892146825d"
            }
          ]
        },
        {
          "id": "0b8323e6-0b7a-45d8-bb57-c5e2de46049c",
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
              "id": "15f22629-9c74-4e8e-b71d-d65b23b0d793"
            }
          ]
        },
        {
          "id": "e83f3dee-b727-4ee6-96a6-67c6054b8d77",
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
              "id": "56aa24a3-b4e1-42a1-987a-0cf649704f60"
            }
          ]
        }
      ]
    },
    {
      "name": "Hostgroups",
      "item": [
        {
          "id": "84331e80-569a-4493-9ce8-11be0f640563",
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
              "id": "e2860721-2665-405c-b438-d50b2bccec9f"
            }
          ]
        },
        {
          "id": "5bbbb4b7-ac55-4d33-b613-53d6fc89a027",
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
              "id": "2814ce2a-21c9-48f6-a65b-65d32760304a"
            }
          ]
        },
        {
          "id": "224906a1-c2ef-4ee5-a21b-25b48058f6b7",
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
              "id": "59661eff-8b8f-4bd4-b579-a301eb42e374"
            }
          ]
        },
        {
          "id": "9d7d046e-a296-46e2-adb9-011ecdfda0dd",
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
              "id": "0212b94e-78b6-4f22-aacc-2f57142a7853"
            }
          ]
        },
        {
          "id": "dc7aa447-b8ee-4f5e-90da-30c61f06d638",
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
              "id": "6199a96c-d5dc-4a75-a927-2108552eba6e"
            }
          ]
        },
        {
          "id": "d14d72b8-bf24-4e41-8380-f512ad33cf6d",
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
              "id": "10895881-f5ee-434e-9b46-b52abc7c0212"
            }
          ]
        }
      ]
    },
    {
      "name": "Meters",
      "item": [
        {
          "id": "ca75bfea-e155-4248-be20-63541ca0481e",
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
              "id": "0b9c0a49-172c-4b77-85a8-9bf37e36b58b"
            }
          ]
        }
      ]
    },
    {
      "name": "Measurements",
      "item": [
        {
          "id": "ff46c607-cd30-41ed-a546-c831b1c9249e",
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
              "id": "a00ae4a6-ef61-4d77-8f5c-43a726e79c57"
            }
          ]
        },
        {
          "id": "dafa4ee3-9823-4ef9-b4ca-2781be224d4a",
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
              "id": "145cbead-6215-4e3e-a913-ff60819e1197"
            }
          ]
        }
      ]
    }
  ]
}