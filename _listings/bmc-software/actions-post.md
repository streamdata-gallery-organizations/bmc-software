---
swagger: "2.0"
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /actions:
    post:
      summary: Create Action
      description: Create a new Action
      operationId: create-action
      parameters:
      - in: path
        name: "action_name\n        \n        \n            required\n            Display
          name for the Action.\n        \n    \n    \n        \n        action_url\n
          \       \n        \n            required\n            URL to be invoked
          for action execution."
      responses:
        200:
          description: OK
      tags:
      - actions
definitions: []
x-collection-name: BMC Software
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---