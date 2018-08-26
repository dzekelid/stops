---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopReplicationTask:
    get:
      summary: Stop Replication Task
      description: Stops the replication task.
      operationId: stopReplicationTask
      x-api-path-slug: actionstopreplicationtask-get
      parameters:
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number(ARN) of the replication task to be
          stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
---