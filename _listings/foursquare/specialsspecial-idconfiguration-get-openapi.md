---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Specials Configuration
  description: /specials/search
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /specials/{SPECIAL_ID}/configuration:
    get:
      summary: Get Specials Configuration
      description: /specials/search
      operationId: specialssearch
      x-api-path-slug: specialsspecial-idconfiguration-get
      parameters:
      - in: query
        name: SPECIAL_ID
        description: The ID of the special to retrieve configuration details for
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
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