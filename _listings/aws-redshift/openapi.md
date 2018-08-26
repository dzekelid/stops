---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisableLogging:
    get:
      summary: Disable Logging
      description: |-
        Stops logging information, such as queries and connection attempts, for the
                    specified Amazon Redshift cluster.
      operationId: disableLogging
      x-api-path-slug: actiondisablelogging-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster on which logging is to be stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging
---