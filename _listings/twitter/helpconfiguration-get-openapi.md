---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Help Configuration
  description: Returns the current configuration used by Twitter including twitter.com
    slugs which are not usernames
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /help/configuration:
    get:
      summary: Help Configuration
      description: Returns the current configuration used by Twitter including twitter.com
        slugs which are not usernames
      operationId: returns-the-current-configuration-used-by-twitter-including-twittercom-slugs-which-are-not-usernames
      x-api-path-slug: helpconfiguration-get
      responses:
        200:
          description: OK
      tags:
      - Help
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