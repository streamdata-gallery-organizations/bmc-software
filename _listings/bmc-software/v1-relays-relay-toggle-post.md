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
  /v1/relays/:relay/toggle:
    post:
      summary: Toggle relay
      description: Set a relay to be disabled or enabled
      operationId: toggle-relay
      parameters:
      - in: formData
        name: disabled
        description: true or false
        type: string
      - in: query
        name: |-
          relay
          Name of relay to toggle
        type: string
      responses:
        200:
          description: OK
      tags:
      - relays
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