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
  /?Action=PutMetricAlarm&k=1:
    "":
      summary: Put Metric Alarm
      description: Creates or updates an alarm and associates it with the specified
        metric
      operationId: putmetricalarm
      parameters:
      - in: query
        name: ActionsEnabled
        description: Indicates whether actions should be executed during any changes
          to the alarm state
        type: string
      - in: query
        name: AlarmActions.member.N
        description: The actions to execute when this alarm transitions to the ALARM
          state from any other state
        type: string
      - in: query
        name: AlarmDescription
        description: The description for the alarm
        type: string
      - in: query
        name: AlarmName
        description: The name for the alarm
        type: string
      - in: query
        name: ComparisonOperator
        description: "The arithmetic operation to use when comparing the specified
          statistic and\t\t\tthreshold"
        type: string
      - in: query
        name: Dimensions.member.N
        description: The dimensions for the metric associated with the alarm
        type: string
      - in: query
        name: EvaluationPeriods
        description: "The number of periods over which data is compared to the specified\t\t\tthreshold"
        type: string
      - in: query
        name: ExtendedStatistic
        description: The percentile statistic for the metric associated with the alarm
        type: string
      - in: query
        name: InsufficientDataActions.member.N
        description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA
          state from any other state
        type: string
      - in: query
        name: MetricName
        description: The name for the metric associated with the alarm
        type: string
      - in: query
        name: Namespace
        description: The namespace for the metric associated with the alarm
        type: string
      - in: query
        name: OKActions.member.N
        description: "The actions to execute when this alarm transitions to an OK
          state\t\t\tfrom any other state"
        type: string
      - in: query
        name: Period
        description: The period, in seconds, over which the specified statistic is
          applied
        type: string
      - in: query
        name: Statistic
        description: The statistic for the metric associated with the alarm, other
          than percentile
        type: string
      - in: query
        name: Threshold
        description: The value against which the specified statistic is compared
        type: string
      - in: query
        name: Unit
        description: The unit of measure for the statistic
        type: string
      responses:
        200:
          description: OK
      tags:
      - alarm metric
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