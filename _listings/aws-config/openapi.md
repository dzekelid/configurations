---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 1
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetResourceConfigHistory:
    get:
      summary: Get Resource Config History
      description: Returns a list of configuration items for the specified resource.
      operationId: getResourceConfigHistory
      x-api-path-slug: actiongetresourceconfighistory-get
      parameters:
      - in: query
        name: chronologicalOrder
        description: The chronological order for configuration items listed
        type: string
      - in: query
        name: earlierTime
        description: The time stamp that indicates an earlier time
        type: string
      - in: query
        name: laterTime
        description: The time stamp that indicates a later time
        type: string
      - in: query
        name: limit
        description: The maximum number of configuration items returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceId
        description: The ID of the resource (for example
        type: string
      - in: query
        name: resourceType
        description: The resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Configurations
---