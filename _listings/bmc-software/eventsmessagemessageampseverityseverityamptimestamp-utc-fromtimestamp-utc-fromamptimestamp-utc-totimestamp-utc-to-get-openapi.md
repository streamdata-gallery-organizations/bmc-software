---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to}
  version: 1.0.0
  description: Gets a list of events for the current user.
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