---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 0
info:
  title: Google App Engine Admin API Get Configuration
  description: Gets the current configuration of the specified service.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps/{appsId}/services/{servicesId}:
    get:
      summary: Get Configuration
      description: Gets the current configuration of the specified service.
      operationId: appengine.apps.services.get
      x-api-path-slug: v1appsappsidservicesservicesid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Configuration
    patch:
      summary: Update Configuration
      description: Updates the configuration of the specified service.
      operationId: appengine.apps.services.patch
      x-api-path-slug: v1appsappsidservicesservicesid-patch
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: migrateTraffic
        description: Set to true to gradually shift traffic to one or more versions
          that you specify
      - in: path
        name: servicesId
        description: Part of `name`
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - Configuration
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