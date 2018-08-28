---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Stop Configuration Recorder
  version: 1.0.0
  description: Stops recording configurations of the AWS resources you have selected
    to record in your AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopConfigurationRecorder:
    get:
      summary: Stop Configuration Recorder
      description: Stops recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: stopConfigurationRecorder
      x-api-path-slug: actionstopconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
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