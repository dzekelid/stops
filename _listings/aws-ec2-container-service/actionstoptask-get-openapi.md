---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Stop Task
  version: 1.0.0
  description: Stops a running task.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopTask:
    get:
      summary: Stop Task
      description: Stops a running task.
      operationId: stopTask
      x-api-path-slug: actionstoptask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the task to stop
        type: string
      - in: query
        name: reason
        description: An optional message specified when a task is stopped
        type: string
      - in: query
        name: task
        description: The task ID or full Amazon Resource Name (ARN) entry of the task
          to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
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