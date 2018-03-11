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
  /?Action=GetMetricStatistics&k=1:
    "":
      summary: Get Metric Statistics
      description: Gets statistics for the specified metric
      operationId: getmetricstatistics
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions
        type: string
      - in: query
        name: EndTime
        description: The time stamp that determines the last data point to return
        type: string
      - in: query
        name: ExtendedStatistics.member.N
        description: The percentile statistics
        type: string
      - in: query
        name: MetricName
        description: The name of the metric, with or without spaces
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric, with or without spaces
        type: string
      - in: query
        name: Period
        description: The granularity, in seconds, of the returned data points
        type: string
      - in: query
        name: StartTime
        description: The time stamp that determines the first data point to return
        type: string
      - in: query
        name: Statistics.member.N
        description: The metric statistics, other than percentile
        type: string
      - in: query
        name: Unit
        description: The unit for a given metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - metric statistics
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