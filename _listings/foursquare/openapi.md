swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
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