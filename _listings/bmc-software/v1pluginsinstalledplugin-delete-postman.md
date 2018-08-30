{
  "info": {
    "name": "BMC Software API Uninstall plugin",
    "_postman_id": "ffde52e5-640e-4fc6-8292-bc8b8ca4b4fa",
    "description": "Uninstalls a plugin and optionally removes related dashboard(s) and metric(s).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Plugins",
      "item": [
        {
          "id": "51727f35-dd44-43be-9323-d00fec7117c8",
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
              "id": "1e81fceb-4248-4f4d-bf60-7efb1bfa009d"
            }
          ]
        },
        {
          "id": "7aacfcf6-06df-47fb-85a8-03391639ef77",
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
              "id": "213e3586-14c1-4ff3-91a4-f15d9d7fb4d6"
            }
          ]
        },
        {
          "id": "1528bad1-22f4-4045-ac21-fe0801f58ea2",
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
              "id": "0e50e07c-ee0e-4997-933c-0231dcb8c6e5"
            }
          ]
        },
        {
          "id": "9e5a8954-ddb4-4bc6-a34c-7103453b05b6",
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
              "id": "3cb238df-10ae-4e24-a4d6-5422c776daf5"
            }
          ]
        },
        {
          "id": "706ad822-93c5-47de-9fdb-1303aa0fe1b5",
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
              "id": "6cedf486-5098-4b0a-86f1-485d56f753d8"
            }
          ]
        },
        {
          "id": "a43e6ce9-3d4b-4df4-bdd6-64aa6e4c2eb6",
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
              "id": "5e841dd6-0313-49a6-b081-396ba024d595"
            }
          ]
        },
        {
          "id": "c90c0779-bdac-4b4a-a3fa-c7597559d181",
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
              "id": "d989d639-ec47-43da-b0d1-c42f410d3985"
            }
          ]
        }
      ]
    }
  ]
}