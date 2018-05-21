{
  "info": {
    "name": "BMC Software API Get plugin components",
    "_postman_id": "cc9f860d-8e55-4c9c-9d19-b56d09e165e9",
    "description": "Finds the components associated with an installed plugin including metrics and dashboards",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Plugins",
      "item": [
        {
          "id": "ebc3ea96-1ae1-429c-8b70-3493c9937428",
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
              "id": "0c1a0202-b55e-43a5-8486-a741f74ae4de"
            }
          ]
        },
        {
          "id": "04a2a900-101a-4263-a014-8836c813e0ad",
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
              "id": "f11cd19e-2fef-46dc-98e1-94f42c773c2d"
            }
          ]
        }
      ]
    }
  ]
}