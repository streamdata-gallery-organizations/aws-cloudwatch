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
  /?Action=DescribeAlarmsForMetric&k=1:
    "":
      summary: Describe Alarms For Metric
      description: Retrieves the alarms for the specified metric
      operationId: describealarmsformetric
      parameters:
      - in: query
        name: Dimensions.member.N
        description: The dimensions associated with the metric
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric
        type: string
      - in: query
        name: MetricName
        description: The name of the metric
        type: string
      - in: query
        name: Namespace
        description: The namespace of the metric
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the statistic is applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric, other than percentiles
        type: string
      - in: query
        name: Unit
        description: The unit for the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - alarm metrics
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