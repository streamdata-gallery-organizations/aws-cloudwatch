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
  /?Action=PutMetricData&k=1:
    "":
      summary: Put Metric Data
      description: Publishes metric data points to Amazon CloudWatch
      operationId: putmetricdata
      parameters:
      - in: query
        name: MetricData.member.N
        description: The data for the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric data
        type: string
      responses:
        200:
          description: OK
      tags:
      - data metric
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