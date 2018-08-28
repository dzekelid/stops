swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 1
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopExecution:
    get:
      summary: Stop Execution
      description: Stops an execution.
      operationId: stopExecution
      x-api-path-slug: actionstopexecution-get
      parameters:
      - in: query
        name: cause
        description: A more detailed explanation of the cause of the termination
        type: string
      - in: query
        name: error
        description: An arbitrary error code that identifies the cause of the termination
        type: string
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Execution