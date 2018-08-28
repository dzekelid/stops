---
swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 0
info:
  title: AWS Kinesis Analytics API Stop Application
  version: 1.0.0
  description: Stops the application from processing input data.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopApplication:
    get:
      summary: Stop Application
      description: Stops the application from processing input data.
      operationId: stopApplication
      x-api-path-slug: actionstopapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the running application to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
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