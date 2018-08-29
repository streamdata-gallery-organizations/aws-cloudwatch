---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Delete Alarms
  version: 1.0.0
  description: Deletes the specified alarms.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteAlarms:
    "":
      summary: Delete Alarms
      description: Deletes the specified alarms.
      operationId: deletealarms
      x-api-path-slug: actiondeletealarms-
      parameters:
      - in: query
        name: AlarmNames.member.N
        description: The alarms to be deleted
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