---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Disable Alarm Actions
  version: 1.0.0
  description: Disables the actions for the specified alarms.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisableAlarmActions:
    "":
      summary: Disable Alarm Actions
      description: Disables the actions for the specified alarms.
      operationId: disablealarmactions
      x-api-path-slug: actiondisablealarmactions-
      parameters:
      - in: query
        name: AlarmNames.member.N
        description: The names of the alarms
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm Actions
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