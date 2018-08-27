---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez If Due Date is not populated a complete flag is set or if Due Date
    is populated a recurrence is set
  version: 1.0.0
  description: If due date is not populated a complete flag is set or if due date
    is populated a recurrence is set.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/completetask:
    put:
      summary: If Due Date is not populated a complete flag is set or if Due Date
        is populated a recurrence is set
      description: If due date is not populated a complete flag is set or if due date
        is populated a recurrence is set.
      operationId: DefaultToDo_CompleteTaskBycompleteTask
      x-api-path-slug: apitodocompletetask-put
      parameters:
      - in: body
        name: completeTask
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - If
      - Due
      - Date
      - Is
      - Not
      - Populated
      - Complete
      - Flag
      - Is
      - Set
      - If
      - Due
      - Date
      - Is
      - Populated
      - Recurrence
      - Is
      - Set
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