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
  /?Action=ListMetrics&k=1:
    "":
      summary: List Metrics
      description: List the specified metrics
      operationId: listmetrics
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions to filter against
        type: string
      - in: query
        name: MetricName
        description: The name of the metric to filter against
        type: string
      - in: query
        name: Namespace
        description: The namespace to filter against
        type: string
      - in: query
        name: NextToken
        description: "The token returned by a previous call to indicate that there
          is more data\t\t\tavailable"
        type: string
      responses:
        200:
          description: OK
      tags:
      - metrics
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