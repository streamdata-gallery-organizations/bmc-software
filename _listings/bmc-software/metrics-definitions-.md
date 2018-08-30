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
  /metrics/definitions:
    "":
      summary: Available metrics
      description: Determine which metrics are available to return historical data
        for, for a specific subject (device or service) over a specific time range
      operationId: available-metrics
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: subjectId
        description: The ID of the subject to get the definitions for, e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - metrics
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