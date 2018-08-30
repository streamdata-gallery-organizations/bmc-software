{
  "info": {
    "name": "BMC Software API Get AWS Integration Status",
    "_postman_id": "8c3ad483-0df9-43e0-88e2-282d9c7ecf1c",
    "description": "Gets AWS status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "cc44394f-c5be-4a08-9af1-4e2196a41dc0",
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
              "id": "da45dfcd-9d52-401f-a807-8fc4ae4a7a96"
            }
          ]
        },
        {
          "id": "4b9ef511-48ea-4218-9897-7a3d5f115bb5",
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
              "id": "fceb1b55-1c9f-4916-a568-eb18e819fa96"
            }
          ]
        }
      ]
    }
  ]
}