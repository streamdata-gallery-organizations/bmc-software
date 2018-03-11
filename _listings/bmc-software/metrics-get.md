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
  /metrics:
    get:
      summary: Get list of active metrics
      description: |2-

                  Get the list of actively reporting metrics from a given time until now
      operationId: get-list-of-active-metrics
      parameters:
      - in: query
        name: '[[POSIX_timestamp, numeric_value], ...]'
        description: "\n              \n              Note that the timestamp should
          be in seconds, must be current, and the numeric value is a 32bit float gauge-type
          value"
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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