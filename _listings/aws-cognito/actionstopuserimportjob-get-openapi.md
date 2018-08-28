---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Stop User Import Job
  version: 1.0.0
  description: Stops the user import job.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopUserImportJob:
    get:
      summary: Stop User Import Job
      description: Stops the user import job.
      operationId: stopUserImportJob
      x-api-path-slug: actionstopuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Iimport
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