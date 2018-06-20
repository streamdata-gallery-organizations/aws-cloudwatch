---
swagger: "2.0"
x-collection-name: AWS CloudWatch
x-complete: 0
info:
  title: Amazon CloudWatch API Describe Alarm History
  version: 1.0.0
  description: Retrieves the history for the specified alarm.
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
  /?Action=DescribeAlarmHistory:
    "":
      summary: Describe Alarm History
      description: Retrieves the history for the specified alarm.
      operationId: describealarmhistory
      x-api-path-slug: actiondescribealarmhistory-
      parameters:
      - in: query
        name: AlarmName
        description: The name of the alarm
        type: string
      - in: query
        name: EndDate
        description: The ending date to retrieve alarm history
        type: string
      - in: query
        name: HistoryItemType
        description: The type of alarm histories to retrieve
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of alarm history records to retrieve
        type: string
      - in: query
        name: NextToken
        description: The token returned by a previous call to indicate that there
          is more dataavailable
        type: string
      - in: query
        name: StartDate
        description: The starting date to retrieve alarm history
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarm History
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