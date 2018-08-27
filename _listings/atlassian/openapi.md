swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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