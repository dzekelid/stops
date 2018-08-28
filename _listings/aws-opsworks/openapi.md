swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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