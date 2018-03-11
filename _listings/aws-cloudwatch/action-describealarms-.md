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
  /?Action=DescribeAlarms&k=1:
    "":
      summary: Describe Alarms
      description: Retrieves the specified alarms
      operationId: describealarms
      parameters:
      - in: query
        name: ActionPrefix
        description: The action name prefix
        type: string
      - in: query
        name: AlarmNamePrefix
        description: The alarm name prefix
        type: string
      - in: query
        name: AlarmNames.member.N
        description: The names of the alarms
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of alarm descriptions to retrieve
        type: string
      - in: query
        name: NextToken
        description: "The token returned by a previous call to indicate that there
          is more data\t\t\tavailable"
        type: string
      - in: query
        name: StateValue
        description: The state value to be used in matching alarms
        type: string
      responses:
        200:
          description: OK
      tags:
      - alarms
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