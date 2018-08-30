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
  /v1/relays/:relay/config:
    get:
      summary: Get Relay Configuration
      description: |-
        Retrieves config for a relay host if changed
        If no timestamp specified, configuration data is always returned
        If config has not changed the string &#39;not-modified&#39; is returned
      operationId: get-relay-configuration
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