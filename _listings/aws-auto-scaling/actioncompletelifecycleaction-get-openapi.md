---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Complete Lifecycle Action
  version: 1.0.0
  description: Completes the lifecycle action for the specified token or instance
    with the specified result.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CompleteLifecycleAction:
    get:
      summary: Complete Lifecycle Action
      description: Completes the lifecycle action for the specified token or instance
        with the specified result.
      operationId: completeLifecycleAction
      x-api-path-slug: actioncompletelifecycleaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group for the lifecycle hook
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: LifecycleActionResult
        description: The action for the group to take
        type: string
      - in: query
        name: LifecycleActionToken
        description: A universally unique identifier (UUID) that identifies a specific
          lifecycle action associated with an instance
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
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