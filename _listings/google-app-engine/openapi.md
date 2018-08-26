---
swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 1
info:
  title: Google App Engine Admin
  description: provisions-and-manages-app-engine-applications-
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
---