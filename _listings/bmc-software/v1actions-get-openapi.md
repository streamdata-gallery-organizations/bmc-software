---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Get all available action types
  version: 1.0.0
  description: Gets all known action types
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Account Resource
      description: Information about the authorized account.
      operationId: information-about-the-authorized-account
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
  ? '/events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to} '
  : ' get ':
      summary: Events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to}
      description: Gets a list of events for the current user.
      operationId: -eventsmessagemessageampseverityseverityamptimestamp-utc-fromtimestamp-utc-fromamptimestamp-utc-toti
      x-api-path-slug: eventsmessagemessageampseverityseverityamptimestamp-utc-fromtimestamp-utc-fromamptimestamp-utc-totimestamp-utc-to-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events ':
    ' post ':
      summary: Custom Events
      description: Creates new custom event.
      operationId: -custom-events-
      x-api-path-slug: custom-events-post
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events/all?fromUtc={fromUtc}&amp;toUtc={toUtc} ':
    ' get ':
      summary: Custom Events
      description: Gets all custom events using optional filter.
      operationId: -custom-events-allfromutcfromutcamptoutctoutc-
      x-api-path-slug: custom-eventsallfromutcfromutcamptoutctoutc-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events/{id} ':
    ' get ':
      summary: Custom_events {id}
      description: Gets custom event by Id.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
    ' put ':
      summary: Custom_events {id}
      description: Updates custom event.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-put
      responses:
        200:
          description: OK
      tags:
      - Custom Events
    ' delete ':
      summary: Custom_events {id}
      description: Deletes custom event.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  /v1/account/aws/status:
    get:
      summary: Get AWS Integration Status
      description: Gets AWS status
      operationId: get-aws-integration-status
      x-api-path-slug: v1accountawsstatus-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/actions:
    get:
      summary: Get all available action types
      description: Gets all known action types
      operationId: get-all-available-action-types
      x-api-path-slug: v1actions-get
      responses:
        200:
          description: OK
      tags:
      - Actions
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