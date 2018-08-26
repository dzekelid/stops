---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
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
      description: Stops a specific Amazon Lightsail instance that is currently running.
      operationId: stopInstance
      x-api-path-slug: actionstopinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance (a virtual private server) to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
---