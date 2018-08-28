swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StopWorkspaces:
    get:
      summary: Stop Workspaces
      description: Stops the specified WorkSpaces.
      operationId: stopWorkspaces
      x-api-path-slug: actionstopworkspaces-get
      parameters:
      - in: query
        name: StopWorkspaceRequests
        description: The requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces