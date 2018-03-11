---
swagger: "2.0"
info:
  title: AWS CloudWatch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetAlarmState&k=1:
    "":
      summary: Set Alarm State
      description: Temporarily sets the state of an alarm for testing purposes
      operationId: setalarmstate
      parameters:
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: StateReason
        description: The reason that this alarm is set to this specific state, in
          text format
        type: string
      - in: query
        name: StateReasonData
        description: The reason that this alarm is set to this specific state, in
          JSON format
        type: string
      - in: query
        name: StateValue
        description: The value of the state
        type: string
      responses:
        200:
          description: OK
      tags:
      - aler state
definitions: []
x-collection-name: AWS CloudWatch
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