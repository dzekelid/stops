---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Stop Stack
  version: 1.0.0
  description: Stops a specified stack.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopInstance:
    get:
      summary: Stop Instance
      description: Stops a specified instance.
      operationId: stopInstance
      x-api-path-slug: actionstopinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Instance
  /?Action=StopStack:
    get:
      summary: Stop Stack
      description: Stops a specified stack.
      operationId: stopStack
      x-api-path-slug: actionstopstack-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Stack
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