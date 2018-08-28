swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
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