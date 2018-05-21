{
  "info": {
    "name": "BMC Software API Get all plugins",
    "_postman_id": "51c88198-5070-45d8-a6ae-15dc7cf1179f",
    "description": "Gets all known plugin definitions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Plugins",
      "item": [
        {
          "id": "fccc38b1-f349-442f-be00-a3cf482c2713",
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
              "id": "09261128-c7e3-44d2-84cd-77fdb2d09a70"
            }
          ]
        }
      ]
    }
  ]
}