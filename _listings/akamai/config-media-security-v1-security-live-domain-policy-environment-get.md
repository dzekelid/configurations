---
swagger: "2.0"
info:
  title: Akamai API Get an HD Config Policy per Environment
  description: Get an HD Config Policy per Environment
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /config-media-security/v1/security/live/{domain}/policy/{environment}:
    get:
      summary: Get an HD Config Policy per Environment
      description: Get an HD Config Policy per Environment
      operationId: configmediasecurityv1securitylivedomainpolicyenvironment
      parameters:
      - in: query
        name: domain
        description: The fully qualified domain name for the host in question
        type: string
      - in: query
        name: environment
        description: The environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - configurations
      - media
      - security
      - security
      - live
      - domain
      - policy
      - environment
definitions: []
x-collection-name: Akamai
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