---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
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
---