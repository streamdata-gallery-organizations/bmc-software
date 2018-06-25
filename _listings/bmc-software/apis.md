---
name: BMC Software
x-slug: bmc-software
description: Transform your digital enterprise with BMC IT solutions. From mainframe
  to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
x-kinRank: "8"
x-alexaRank: "27308"
tags: BMC Software
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software API Account Resource
  x-api-slug: bmc-software-api
  description: Information about the authorized account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///account
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/account-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/account-get-openapi.md
- name: BMC Software API Events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to}
  x-api-slug: bmc-software-api
  description: Gets a list of events for the current user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to} '
  tags: Custom Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/eventsmessagemessageampseverityseverityamptimestamp-utc-fromtimestamp-utc-fromamptimestamp-utc-totimestamp-utc-to-get-openapi.md
- name: BMC Software API Custom Events
  x-api-slug: bmc-software-api
  description: Creates new custom event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///custom_events '
  tags: Custom Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-events-post-openapi.md
- name: BMC Software API Custom_events All?fromUtc={fromUtc}&amp;toUtc={toUtc}
  x-api-slug: bmc-software-api
  description: Gets all custom events using optional filter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///custom_events/all?fromUtc={fromUtc}&amp;toUtc={toUtc} '
  tags: Custom Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsallfromutcfromutcamptoutctoutc-get-openapi.md
- name: BMC Software API Custom_events {id}
  x-api-slug: bmc-software-api
  description: Gets custom event by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///custom_events/{id} '
  tags: Custom Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-get-openapi.md
- name: BMC Software API Custom_events {id}
  x-api-slug: bmc-software-api
  description: Updates custom event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///custom_events/{id} '
  tags: Custom Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-put-openapi.md
- name: BMC Software API Custom_events {id}
  x-api-slug: bmc-software-api
  description: Deletes custom event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: 'https://///custom_events/{id} '
  tags: Custom Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/custom-eventsid-delete-openapi.md
- name: BMC Software API Get AWS Integration Status
  x-api-slug: bmc-software-api
  description: Gets AWS status
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/account/aws/status
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountawsstatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountawsstatus-get-openapi.md
- name: BMC Software API Get all available action types
  x-api-slug: bmc-software-api
  description: Gets all known action types
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actions-get-openapi.md
- name: BMC Software API Get all installed actions
  x-api-slug: bmc-software-api
  description: Gets all actions that are installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalled-get-openapi.md
- name: BMC Software API Install action
  x-api-slug: bmc-software-api
  description: Installs an action
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalled-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalled-put-openapi.md
- name: BMC Software API Get details of an installed action
  x-api-slug: bmc-software-api
  description: Gets a single action definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionid-get-openapi.md
- name: BMC Software API Get all alarms using an action
  x-api-slug: bmc-software-api
  description: Get alarms that are using this action installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId/alarms
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionidalarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionidalarms-get-openapi.md
- name: BMC Software API Uninstall action
  x-api-slug: bmc-software-api
  description: Uninstalls an action and remove it from the associated alarms(s).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsinstalledactionid-delete-openapi.md
- name: BMC Software API Get action
  x-api-slug: bmc-software-api
  description: Gets a single action type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/:action
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsaction-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1actionsaction-get-openapi.md
- name: BMC Software API Get All Alarms
  x-api-slug: bmc-software-api
  description: Get all of the Alarms
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarms-get-openapi.md
- name: BMC Software API Get Alarm by Id
  x-api-slug: bmc-software-api
  description: Retrieves a single alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmalarmid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmalarmid-get-openapi.md
- name: BMC Software API Get Alarms by Name
  x-api-slug: bmc-software-api
  description: Retrieves alarms by name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms/search
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmssearch-get-openapi.md
- name: BMC Software API Create Alarm
  x-api-slug: bmc-software-api
  description: Create an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarms-post-openapi.md
- name: BMC Software API Update Alarm
  x-api-slug: bmc-software-api
  description: Update an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmalarmid-put-openapi.md
- name: BMC Software API Delete Alarm
  x-api-slug: bmc-software-api
  description: Deletes an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/alarm/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1alarmalarmid-delete-openapi.md
- name: BMC Software API Create Alarm
  x-api-slug: bmc-software-api
  description: Create an Alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarms-post-openapi.md
- name: BMC Software API Update Alarm
  x-api-slug: bmc-software-api
  description: Updates an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarmsalarmid-put-openapi.md
- name: BMC Software API Get All Alarms
  x-api-slug: bmc-software-api
  description: Get all of the Alarms
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarms-get-openapi.md
- name: BMC Software API Get Alarm by Id
  x-api-slug: bmc-software-api
  description: Retrieves a single alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarmsalarmid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarmsalarmid-get-openapi.md
- name: BMC Software API Delete Alarm
  x-api-slug: bmc-software-api
  description: Deletes an alarm
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v2/alarms/:alarmId
  tags: Alarms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v2alarmsalarmid-delete-openapi.md
- name: BMC Software API Perform batch
  x-api-slug: bmc-software-api
  description: |-
    Allows making an arbitrary set of API calls.    All calls are made in parallel.
    The query string parameter <em>?series</em> can be used to override this behavior and call the API in series stopping at the first error.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/batch
  tags: Batch
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batch-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batch-post-openapi.md
- name: BMC Software API Delete Mobile Device
  x-api-slug: bmc-software-api
  description: Deletes a device from a user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/mobile-devices/:userDeviceId
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1mobiledevicesuserdeviceid-delete-openapi.md
- name: BMC Software API Delete Account Mobile Device
  x-api-slug: bmc-software-api
  description: Deletes a device from an account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/account/mobile-devices/:accountDeviceId
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountmobiledevicesaccountdeviceid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountmobiledevicesaccountdeviceid-delete-openapi.md
- name: BMC Software API Get All Account Mobile Devices
  x-api-slug: bmc-software-api
  description: Gets all of the devices for an account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/account/mobile-devices
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountmobiledevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountmobiledevices-get-openapi.md
- name: BMC Software API List dataset
  x-api-slug: bmc-software-api
  description: '*'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/datasets/*
  tags: Datasets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1datasets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1datasets-get-openapi.md
- name: BMC Software API Create event
  x-api-slug: bmc-software-api
  description: Creates an event. Every event occurrence is persisted to the database
    as a RawEvent. Based on the EventFingerprint, a new Event will be created or an
    existing one will be de-duplicated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/events
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1events-post-openapi.md
- name: BMC Software API List raw events
  x-api-slug: bmc-software-api
  description: Queries all event occurrences (raw events) for the specified organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/events/raw
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsraw-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsraw-get-openapi.md
- name: BMC Software API List events
  x-api-slug: bmc-software-api
  description: Searches for events in the specified organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/events
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1events-get-openapi.md
- name: BMC Software API Get event
  x-api-slug: bmc-software-api
  description: Returns the event with the specified event id from the database.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/events/:event_id
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsevent-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsevent-id-get-openapi.md
- name: BMC Software API Get raw events
  x-api-slug: bmc-software-api
  description: Returns all of the event occurrences (raw events) for the specified
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/events/:event_id/raw
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsevent-idraw-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1eventsevent-idraw-get-openapi.md
- name: BMC Software API Get All Hostgroups
  x-api-slug: bmc-software-api
  description: Get all of the Hostgroups in your account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups
  tags: Hostgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroups-get-openapi.md
- name: BMC Software API Search Hostgroups
  x-api-slug: bmc-software-api
  description: Searches the hostgroups in your account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups/search
  tags: Hostgroups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroupssearch-get-openapi.md
- name: BMC Software API Get Hostgroup by Id
  x-api-slug: bmc-software-api
  description: Retrieves a single hostgroup by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups/:hostgroupId
  tags: Hostgroups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroupshostgroupid-get-openapi.md
- name: BMC Software API Create Hostgroup
  x-api-slug: bmc-software-api
  description: Create a Hostgroup
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups
  tags: Hostgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroups-post-openapi.md
- name: BMC Software API Update Hostgroup
  x-api-slug: bmc-software-api
  description: Update a Hostgroup
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups/:hostgroupId
  tags: Hostgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroupshostgroupid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroupshostgroupid-put-openapi.md
- name: BMC Software API Delete Hostgroup
  x-api-slug: bmc-software-api
  description: Delete an hostgroup
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/hostgroups/:hostgroupId
  tags: Hostgroups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1hostgroupshostgroupid-delete-openapi.md
- name: BMC Software API Registration
  x-api-slug: bmc-software-api
  description: Register a Meter with TrueSight Pulse
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/meter/:meterName/registration
  tags: Meters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metermeternameregistration-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metermeternameregistration-post-openapi.md
- name: BMC Software API Add measures
  x-api-slug: bmc-software-api
  description: Adds measurement readings to the data store.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/measurements
  tags: Measurements
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurements-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurements-post-openapi.md
- name: BMC Software API Create metric
  x-api-slug: bmc-software-api
  description: Creates a new metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metrics-post-openapi.md
- name: BMC Software API Create metrics batch
  x-api-slug: bmc-software-api
  description: Creates metrics, but in a batch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/batch/metrics
  tags: Batch
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batchmetrics-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batchmetrics-post-openapi.md
- name: BMC Software API Get measures
  x-api-slug: bmc-software-api
  description: Retrieves measurement readings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/measurements/:metric
  tags: Measurements
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurementsmetric-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurementsmetric-get-openapi.md
- name: BMC Software API Get measures batch
  x-api-slug: bmc-software-api
  description: Same as /v1/measurements/:metric except that an array of query objects
    are passed in the body.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/measurementsBatch
  tags: Measurements
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurementsbatch-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1measurementsbatch-post-openapi.md
- name: BMC Software API Get Metrics
  x-api-slug: bmc-software-api
  description: Retrieves the list of metrics in a project.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metrics-get-openapi.md
- name: BMC Software API Remove metric
  x-api-slug: bmc-software-api
  description: |-
    Removes a metric from the account.
     Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>
     flag is added.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/:metric
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsmetric-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsmetric-delete-openapi.md
- name: BMC Software API Get actions for a dashboard
  x-api-slug: bmc-software-api
  description: |-
    Retrieves the needed configuration changes for a dashboard
     Returns an an array of objects, each has the following properties:
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/dashactions/:dashboardSetId
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-get-openapi.md
- name: BMC Software API Perform dashboard actions
  x-api-slug: bmc-software-api
  description: |-
    Performs necessary actions for a dashboard.
     Only enables or adds metrics at this time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/dashactions/:dashboardSetId
  tags: Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsdashactionsdashboardsetid-post-openapi.md
- name: BMC Software API Update metric
  x-api-slug: bmc-software-api
  description: Updates a metric
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/metrics/:metricName
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1metricsmetricname-put-openapi.md
- name: BMC Software API Update metrics batch
  x-api-slug: bmc-software-api
  description: Updates a batch of metrics
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/batch/metrics
  tags: Batch
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batchmetrics-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1batchmetrics-put-openapi.md
- name: BMC Software API Get all plugins
  x-api-slug: bmc-software-api
  description: Gets all known plugin definitions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1plugins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1plugins-get-openapi.md
- name: BMC Software API Get plugin components
  x-api-slug: bmc-software-api
  description: Finds the components associated with an installed plugin including
    metrics and dashboards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/:plugin/components
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsplugincomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsplugincomponents-get-openapi.md
- name: BMC Software API Get installed plugins
  x-api-slug: bmc-software-api
  description: Gets plugins that are installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalled-get-openapi.md
- name: BMC Software API Install or update plugin
  x-api-slug: bmc-software-api
  description: Installs a plugin
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed/:plugin
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalledplugin-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalledplugin-put-openapi.md
- name: BMC Software API Add private plugin
  x-api-slug: bmc-software-api
  description: |-
    Adds or updates a private plugin.
    A plugin exists as a repository in Github.
    By adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which
    can then be installed and/or added to a relay.
    If a private plugin has the same name as an existing plugin it will override the existing plugin within your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/private/:plugin/:org/:repo
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsprivatepluginorgrepo-put-openapi.md
- name: BMC Software API Remove private plugin
  x-api-slug: bmc-software-api
  description: |-
    Removes a private plugin from your account. Use this function after adding a private plugin to make your private
    plugin disappear from available plugins in your settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/private/:plugin
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsprivateplugin-delete-openapi.md
- name: BMC Software API Uninstall plugin
  x-api-slug: bmc-software-api
  description: Uninstalls a plugin and optionally removes related dashboard(s) and
    metric(s).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed/:plugin
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-openapi.md
- name: BMC Software API Get plugin
  x-api-slug: bmc-software-api
  description: Gets a single plugin definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/:plugin
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1pluginsplugin-get-openapi.md
- name: BMC Software API Set Relay Heartbeat
  x-api-slug: bmc-software-api
  description: |-
    Updates the &#39;lastHeardFrom&#39; field of the relay configuration
    Returns the current system time in UNIX epoch of server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/heartbeat
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysheartbeat-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysheartbeat-post-openapi.md
- name: BMC Software API Get All Relay Configurations
  x-api-slug: bmc-software-api
  description: Gets the configurations for all visible relays
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relays-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relays-get-openapi.md
- name: BMC Software API Get Relay Configuration
  x-api-slug: bmc-software-api
  description: |-
    Retrieves config for a relay host if changed
    If no timestamp specified, configuration data is always returned
    If config has not changed the string &#39;not-modified&#39; is returned
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/config
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayconfig-get-openapi.md
- name: BMC Software API Set Relay Configuration
  x-api-slug: bmc-software-api
  description: |-
    Stores configuration for a relay.
     The relay will gather the configuration on the next poll and reconfigure itself as needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/config
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayconfig-put-openapi.md
- name: BMC Software API Toggle relay
  x-api-slug: bmc-software-api
  description: Set a relay to be disabled or enabled
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/toggle
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelaytoggle-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelaytoggle-post-openapi.md
- name: BMC Software API Toggle relay plugin
  x-api-slug: bmc-software-api
  description: Sets a relay plugin to be disabled or enabled
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/togglePlugin
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelaytoggleplugin-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelaytoggleplugin-post-openapi.md
- name: BMC Software API Add relay output
  x-api-slug: bmc-software-api
  description: |-
    Adds output messages to the relay.
    Used by the relay to communicate output from execution and commands
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/output
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutput-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutput-post-openapi.md
- name: BMC Software API Get relay output
  x-api-slug: bmc-software-api
  description: Queries for relay output messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/output/:since
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutputsince-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutputsince-get-openapi.md
- name: BMC Software API Clear relay output
  x-api-slug: bmc-software-api
  description: Wipes the logged output from the relay up to present.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/relays/:relay/output
  tags: Relays
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutput-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1relaysrelayoutput-delete-openapi.md
- name: BMC Software API Remove Old Sources By Name
  x-api-slug: bmc-software-api
  description: Remove Old Sources from your account by using a list of names
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/sources/byName
  tags: Sources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1sourcesbyname-delete-openapi.md
- name: BMC Software API Get all source information
  x-api-slug: bmc-software-api
  description: Gets all source (host + data stream) information
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/account/sources/:lastModified?
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountsourceslastmodified-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountsourceslastmodified-get-openapi.md
- name: BMC Software API Set source metadata
  x-api-slug: bmc-software-api
  description: Sets one or more source metadata
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///v1/account/sources
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountsources-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/v1accountsources-put-openapi.md
- name: BMC Software API Get list of active metrics
  x-api-slug: bmc-software-api
  description: Get the list of actively reporting metrics from a given time until
    now. This endpoint is not available in the Python and Ruby libraries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///metrics
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/metrics-get-openapi.md
- name: BMC Software API Post an Event
  x-api-slug: bmc-software-api
  description: This end point allows you to post events to the stream. You can tag
    them, set priority and event aggregate them with other events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///api/v1/events
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/apiv1events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/apiv1events-post-openapi.md
- name: BMC Software API Get Actions (Alerts) List
  x-api-slug: bmc-software-api
  description: Returns a list of actions (alerts) that have been generated for your
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: |-
    https:////
        /api/{version}/actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/apiversionactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/apiversionactions-get-openapi.md
- name: BMC Software API Available metrics
  x-api-slug: bmc-software-api
  description: Determine which metrics are available to return historical data for,
    for a specific subject (device or service) over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///metrics/definitions
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/metricsdefinitions--openapi.md
- name: BMC Software API Dynamic metrics
  x-api-slug: bmc-software-api
  description: Return historical metrics data, for a devices and/or services that
    match a search or regex style inventory filter search over a specific time range.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///metrics/dynamicgraphs/
  tags: Metrics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/metricsdynamicgraphs--openapi.md
- name: BMC Software API Create Action
  x-api-slug: bmc-software-api
  description: Create a new Action.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actions-post-openapi.md
- name: BMC Software API Update Action
  x-api-slug: bmc-software-api
  description: Update an existing Action.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///actions/{action_id}
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actionsaction-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actionsaction-id-put-openapi.md
- name: BMC Software API List Actions
  x-api-slug: bmc-software-api
  description: List of all Actions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https://///actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/actions-get-openapi.md
- name: BMC Software API
  x-api-slug: bmc-software-api
  description: Transform your digital enterprise with BMC IT solutions. From mainframe
    to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: BMC Software
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/bmc-software/master/_listings/bmc-software/openapi.md
x-common:
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/bmc
- type: x-documentation
  url: https://docs.bmc.com/docs/dashboard.action
- type: x-email
  url: customer_support@bmc.com
- type: x-email
  url: NA_Accounts_Payable@bmc.com
- type: x-email
  url: Collections_NA@bmc.com
- type: x-email
  url: education@bmc.com
- type: x-email
  url: investor@bmc.com
- type: x-email
  url: global_security@bmc.com
- type: x-email
  url: Compliance_EthicsOffice@bmc.com
- type: x-email
  url: 26Ethics@bmc.com
- type: x-email
  url: Community_Relations@bmc.com
- type: x-github
  url: https://github.com/bmcsoftware
- type: x-twitter
  url: https://twitter.com/bmcsoftware
- type: x-website
  url: http://www.bmc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---