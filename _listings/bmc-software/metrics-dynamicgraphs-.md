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
  /metrics/dynamicgraphs/:
    "":
      summary: Dynamic metrics
      description: Return historical metrics data, for a devices and/or services that
        match a search or regex style inventory filter search over a specific time
        range
      operationId: dynamic-metrics
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: ids
        description: List of inventory IDs
        type: string
      - in: query
        name: inventoryFilter
        description: A regular expression that will return all devices or services
          that match the pattern
        type: string
      - in: query
        name: names
        description: Human-readable names of a device or service
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      - in: query
        name: type
        description: Specify whether to return only devices, services or all
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