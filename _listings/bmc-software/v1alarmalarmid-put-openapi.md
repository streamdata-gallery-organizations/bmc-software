---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Update Alarm
  version: 1.0.0
  description: Update an Alarm
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
  /v1/actions/installed:
    get:
      summary: Get all installed actions
      description: Gets all actions that are installed for the project
      operationId: get-all-installed-actions
      x-api-path-slug: v1actionsinstalled-get
      responses:
        200:
          description: OK
      tags:
      - Actions
    put:
      summary: Install action
      description: Installs an action
      operationId: install-action
      x-api-path-slug: v1actionsinstalled-put
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId:
    get:
      summary: Get details of an installed action
      description: Gets a single action definition
      operationId: get-details-of-an-installed-action
      x-api-path-slug: v1actionsinstalledactionid-get
      parameters:
      - in: query
        name: |-
          actionId
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
    delete:
      summary: Uninstall action
      description: Uninstalls an action and remove it from the associated alarms(s).
      operationId: uninstall-action
      x-api-path-slug: v1actionsinstalledactionid-delete
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId/alarms:
    get:
      summary: Get all alarms using an action
      description: Get alarms that are using this action installed for the project
      operationId: get-all-alarms-using-an-action
      x-api-path-slug: v1actionsinstalledactionidalarms-get
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/:action:
    get:
      summary: Get action
      description: Gets a single action type
      operationId: get-action
      x-api-path-slug: v1actionsaction-get
      parameters:
      - in: query
        name: |-
          action
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/alarms:
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v1alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v1alarms-post
      parameters:
      - in: formData
        name: name
        description: The name of the alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarm/:alarmId:
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v1alarmalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    put:
      summary: Update Alarm
      description: Update an Alarm
      operationId: update-alarm
      x-api-path-slug: v1alarmalarmid-put
      parameters:
      - in: formData
        name: name
        description: The name of the alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarms/search:
    get:
      summary: Get Alarms by Name
      description: Retrieves alarms by name
      operationId: get-alarms-by-name
      x-api-path-slug: v1alarmssearch-get
      parameters:
      - in: query
        name: alarmName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
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