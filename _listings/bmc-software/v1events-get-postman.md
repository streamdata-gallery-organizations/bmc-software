{
  "info": {
    "name": "BMC Software API List events",
    "_postman_id": "6e20886d-e171-4f6b-98d5-b834d4063c50",
    "description": "Searches for events in the specified organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "4ea1d6b1-dd03-4fb0-9385-1c27866c4511",
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
              "id": "fd32a5e7-3f99-49a3-8ef1-297a7185cefb"
            }
          ]
        },
        {
          "id": "0ada2cc8-0ade-4c10-852c-2dfab83638ad",
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
              "id": "408e8e9a-01ea-4622-b807-3ad9daa6178a"
            }
          ]
        },
        {
          "id": "dfa00a7c-b5aa-4edf-82f3-dfebbd95da5e",
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
              "id": "d11a708f-74b7-4a2f-9feb-742477996db5"
            }
          ]
        },
        {
          "id": "dcaecfde-f62a-47d5-acd2-37689768e600",
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
              "id": "3d17d815-17b6-4f62-b2db-107af6f5a1d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Actions",
      "item": [
        {
          "id": "775ae666-0d73-4d2b-bce7-5c12987f7575",
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
              "id": "6416cba6-612f-4973-a60b-dad08d930e1b"
            }
          ]
        },
        {
          "id": "2ce157f0-cf52-4b49-907b-dcd461907132",
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
              "id": "bde6bd1c-cb86-4359-b310-87f83f942f4a"
            }
          ]
        },
        {
          "id": "942c84b6-1da7-4234-9566-e9af4407ce87",
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
              "id": "ca6e3b08-cfab-4c83-985f-fafd60094609"
            }
          ]
        },
        {
          "id": "f77efbda-3a40-434e-b664-5a27448cbad3",
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
              "id": "3baa8309-f981-4c92-ac74-da156e564406"
            }
          ]
        },
        {
          "id": "7300c0a7-6761-4b07-ad25-1a5516138380",
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
              "id": "a1976989-ffc4-48dc-b94a-465fd61816ae"
            }
          ]
        },
        {
          "id": "06a01807-7c4a-45e9-8538-acb073b1a841",
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
              "id": "091034c9-7cd7-4386-80ce-ce3a41650f71"
            }
          ]
        },
        {
          "id": "2e51f979-ee08-4af6-b183-83241ef54548",
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
              "id": "dc5d2d6f-b753-4167-961a-6fed322a9d2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Alarms",
      "item": [
        {
          "id": "83e5690d-9b02-4949-a193-5b03e344865f",
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
              "id": "537d3db8-e711-4740-984f-ac97c7884fa9"
            }
          ]
        },
        {
          "id": "fec5ce3a-8042-44b1-a3af-e8910bb993ec",
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
              "id": "0157d773-a301-4527-8e8f-05e252d380d5"
            }
          ]
        },
        {
          "id": "16dcd02c-d362-4d92-a48b-0651323e147c",
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
              "id": "b5bdba0b-b0c2-4c7f-a988-c457ff1d575a"
            }
          ]
        },
        {
          "id": "79067a24-4f74-4651-922e-154e7b5ad174",
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
              "id": "3002a561-3d43-415f-b5c2-20e2dfa77e65"
            }
          ]
        },
        {
          "id": "94ebddf8-5d02-4b14-9858-3fda3b84469e",
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
              "id": "7a8e338d-5c7d-46ae-abad-4bf5e40812f2"
            }
          ]
        },
        {
          "id": "42aa8be9-0c45-4a46-9da6-dc191e4f69a1",
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
              "id": "5c1eb5f0-7356-4926-8cf6-f579e672dab0"
            }
          ]
        },
        {
          "id": "5e8a324f-8914-463b-9802-10cda11e9377",
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
              "id": "aa230079-69c5-4fe2-82fb-60323271221d"
            }
          ]
        },
        {
          "id": "ec48b59a-134c-445c-95bb-d927e148b763",
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
              "id": "570e05eb-f20f-4511-bca1-5c8af0e595b0"
            }
          ]
        },
        {
          "id": "b0463253-e78a-41af-ae26-4d40852ebf68",
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
              "id": "646e8164-e5a0-46bb-98c4-fa10a522c602"
            }
          ]
        },
        {
          "id": "0071cb0c-0df1-4e62-a395-63c19546bf30",
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
              "id": "3aea6a72-1395-4879-be06-3c8947fd33d8"
            }
          ]
        },
        {
          "id": "28819474-e850-4a77-b489-52519068283c",
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
              "id": "4fa5dbce-d4c2-4057-a21d-ea1db248cb63"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "efa8a107-092a-49e1-8499-9e1f2a6b0138",
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
              "id": "9f8d3c13-4050-48ea-bbda-dfad9b2f6bde"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics",
      "item": [
        {
          "id": "113268a3-4a94-4e7b-9f18-b6c832a9ca5c",
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
              "id": "ec991d3b-8c75-499e-b05c-f431243a069c"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "5c5b95f8-cd9a-4a12-b4ec-0e93b12b37ee",
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
              "id": "cfc8a32f-8b0a-4768-8e1f-be199f14dfbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "27fb1773-0beb-4270-be8c-47c638e3e83b",
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
              "id": "f0dabbda-48bc-4cf7-b8d4-33cc8863de5a"
            }
          ]
        },
        {
          "id": "7bc69fbf-a602-45ea-9b2a-fc5135223c74",
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
              "id": "27cd6b08-50c6-4b0c-9b3c-d20f78afbe40"
            }
          ]
        },
        {
          "id": "cf298a31-270f-420e-b390-7d1c1b9dfa10",
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
              "id": "303dd67e-932a-4173-a155-27d0dc652b94"
            }
          ]
        }
      ]
    }
  ]
}