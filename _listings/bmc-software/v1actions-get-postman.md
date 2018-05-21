{
  "info": {
    "name": "BMC Software API Get all available action types",
    "_postman_id": "077c53fc-300d-4604-8033-02dc1316955c",
    "description": "Gets all known action types",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "8a93598e-5e0c-4e7a-9b11-b56a24fadf19",
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
              "id": "0eae9a24-bf07-4cf5-935b-06e1f1844fd8"
            }
          ]
        }
      ]
    }
  ]
}