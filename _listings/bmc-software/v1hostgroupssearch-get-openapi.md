---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Search Hostgroups
  version: 1.0.0
  description: Searches the hostgroups in your account
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
      summary: Custom_events All?fromUtc={fromUtc}&amp;toUtc={toUtc}
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
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v1alarmalarmid-delete
      parameters:
      - in: query
        name: |-
          alarmId
          The alarm to delete
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
  /v2/alarms:
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v2alarms-post
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v2alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v2/alarms/:alarmId:
    put:
      summary: Update Alarm
      description: Updates an alarm
      operationId: update-alarm
      x-api-path-slug: v2alarmsalarmid-put
      parameters:
      - in: query
        name: |-
          alarmId integer
          The alarm to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v2alarmsalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v2alarmsalarmid-delete
      parameters:
      - in: query
        name: |-
          alarmId
          The alarm to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/batch:
    post:
      summary: Perform batch
      description: |-
        Allows making an arbitrary set of API calls.    All calls are made in parallel.
        The query string parameter <em>?series</em> can be used to override this behavior and call the API in series stopping at the first error.
      operationId: perform-batch
      x-api-path-slug: v1batch-post
      responses:
        200:
          description: OK
      tags:
      - Batch
  /v1/mobile-devices/:userDeviceId:
    delete:
      summary: Delete Mobile Device
      description: Deletes a device from a user
      operationId: delete-mobile-device
      x-api-path-slug: v1mobiledevicesuserdeviceid-delete
      parameters:
      - in: query
        name: |-
          userDeviceId
          The user device ID to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/account/mobile-devices/:accountDeviceId:
    delete:
      summary: Delete Account Mobile Device
      description: Deletes a device from an account
      operationId: delete-account-mobile-device
      x-api-path-slug: v1accountmobiledevicesaccountdeviceid-delete
      parameters:
      - in: query
        name: |-
          accountDeviceId
          The account device ID to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/account/mobile-devices:
    get:
      summary: Get All Account Mobile Devices
      description: Gets all of the devices for an account
      operationId: get-all-account-mobile-devices
      x-api-path-slug: v1accountmobiledevices-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/datasets/*:
    get:
      summary: List dataset
      description: '*'
      operationId: list-dataset
      x-api-path-slug: v1datasets-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /v1/events:
    post:
      summary: Create event
      description: Creates an event. Every event occurrence is persisted to the database
        as a RawEvent. Based on the EventFingerprint, a new Event will be created
        or an existing one will be de-duplicated.
      operationId: create-event
      x-api-path-slug: v1events-post
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: List events
      description: Searches for events in the specified organization.
      operationId: list-events
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/raw:
    get:
      summary: List raw events
      description: Queries all event occurrences (raw events) for the specified organization.
      operationId: list-raw-events
      x-api-path-slug: v1eventsraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id:
    get:
      summary: Get event
      description: Returns the event with the specified event id from the database.
      operationId: get-event
      x-api-path-slug: v1eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id/raw:
    get:
      summary: Get raw events
      description: Returns all of the event occurrences (raw events) for the specified
        event.
      operationId: get-raw-events
      x-api-path-slug: v1eventsevent-idraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/hostgroups:
    get:
      summary: Get All Hostgroups
      description: Get all of the Hostgroups in your account
      operationId: get-all-hostgroups
      x-api-path-slug: v1hostgroups-get
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/hostgroups/search:
    get:
      summary: Search Hostgroups
      description: Searches the hostgroups in your account
      operationId: search-hostgroups
      x-api-path-slug: v1hostgroupssearch-get
      parameters:
      - in: query
        name: |-
          name
          The hostgroup name to search for.  Currently supported search parameters:

          name - search by the name of the hostgroup
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
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