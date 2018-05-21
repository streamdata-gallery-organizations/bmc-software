{
  "info": {
    "name": "BMC Software API Install or update plugin",
    "_postman_id": "12108c4c-3a48-4f52-adf2-db9f3ef62e3b",
    "description": "Installs a plugin",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Plugins",
      "item": [
        {
          "id": "4a6d3a03-6370-4f83-b494-a828a4d4a25e",
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
              "id": "a9464bea-9c4d-4b44-a469-245fbf1cf2cc"
            }
          ]
        },
        {
          "id": "44e16daf-b04a-4d54-8666-1b95180193f2",
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
              "id": "329a0b65-14f7-4ee4-a20c-e95e5b7f19f4"
            }
          ]
        },
        {
          "id": "bbddf16b-9bde-4b46-be11-d382f190ea10",
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
              "id": "832e28b3-bc1a-4ed9-8927-6d77173f5442"
            }
          ]
        },
        {
          "id": "b4c4abd7-6246-441c-bd93-1d4262c6db6b",
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
              "id": "80a069c1-c884-47d1-b963-0a90b10d4e28"
            }
          ]
        }
      ]
    }
  ]
}