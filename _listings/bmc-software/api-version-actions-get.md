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
  ? |2-

        /api/{version}/actions
  : get:
      summary: Get Actions (Alerts) List
      description: |2-

            Returns a list of actions (alerts) that have been generated for your account
      operationId: get-actions-alerts-list
      parameters:
      - in: query
        name: checkids
        description: Comma-separated list of check identifiers
        type: <td>string</td>
      - in: query
        name: contactids
        description: Comma-separated list of contact identifiers
        type: <td>string</td>
      - in: query
        name: from
        description: Only include actions generated later than this timestamp
        type: <td>integer</td>
      - in: query
        name: limit
        description: Limits the number of returned results to the specified quantity
        type: <td>integer (max 300)</td>
      - in: query
        name: offset
        description: Offset for listing
        type: <td>integer</td>
      - in: query
        name: status
        description: Comma-separated list of statuses
        type: <td>string (sent, delivered, error, not_deliv
      - in: query
        name: to
        description: Only include actions generated prior to this timestamp
        type: <td>integer</td>
      - in: query
        name: via
        description: Comma-separated list of via mediums
        type: <td>string (email, sms, twitter, iphone, andr
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