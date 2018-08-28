---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Stop Assessment Run
  version: 1.0.0
  description: |-
    Stops the assessment run that is specified by the ARN of the assessment
             run.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopAssessmentRun:
    get:
      summary: Stop Assessment Run
      description: |-
        Stops the assessment run that is specified by the ARN of the assessment
                 run.
      operationId: stopAssessmentRun
      x-api-path-slug: actionstopassessmentrun-get
      parameters:
      - in: query
        name: assessmentRunArn
        description: The ARN of the assessment run that you want to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
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