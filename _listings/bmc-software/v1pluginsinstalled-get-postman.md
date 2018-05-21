{
  "info": {
    "name": "BMC Software API Get installed plugins",
    "_postman_id": "e38f5d1e-7465-44ff-8bcd-273dd470b295",
    "description": "Gets plugins that are installed for the project",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Plugins",
      "item": [
        {
          "id": "5727c71b-f0a4-476a-9161-443485eaf714",
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
              "id": "d3f860b8-d262-47a2-931b-72fa11e4f73f"
            }
          ]
        },
        {
          "id": "6d1c8baa-8da7-493a-92a1-6aa2d75a2c42",
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
              "id": "46645def-1d5f-43a5-8000-9bf3aaf4af41"
            }
          ]
        },
        {
          "id": "577f60f5-095a-42ac-8871-d01eaf5ebcfd",
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
              "id": "d3d5af8b-2de6-4dfe-87dc-333342a03908"
            }
          ]
        }
      ]
    }
  ]
}