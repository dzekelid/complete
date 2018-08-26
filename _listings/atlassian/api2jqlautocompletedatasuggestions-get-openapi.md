---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get field auto complete for query string
  description: Returns auto complete suggestions for JQL search.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/jql/autocompletedata:
    get:
      summary: Get auto complete
      description: Returns the auto complete data required for JQL searches.
      operationId: com.atlassian.jira.rest.v2.search.SearchAutoCompleteResource.getAutoComplete_get
      x-api-path-slug: api2jqlautocompletedata-get
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Complete
  /api/2/jql/autocompletedata/suggestions:
    get:
      summary: Get field auto complete for query string
      description: Returns auto complete suggestions for JQL search.
      operationId: com.atlassian.jira.rest.v2.search.SearchAutoCompleteResource.getFieldAutoCompleteForQueryString_get
      x-api-path-slug: api2jqlautocompletedatasuggestions-get
      parameters:
      - in: query
        name: fieldName
        description: the field name for which the suggestions are generated
      - in: query
        name: fieldValue
        description: the portion of the field value that has already been provided
          by the user
      - in: query
        name: predicateName
        description: the predicate for which the suggestions are generated
      - in: query
        name: predicateValue
        description: the portion of the predicate value that has already been provided
          by the user
      responses:
        200:
          description: OK
      tags:
      - Field
      - Auto
      - Completequery
      - String
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