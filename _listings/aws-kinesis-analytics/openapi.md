swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 1
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
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