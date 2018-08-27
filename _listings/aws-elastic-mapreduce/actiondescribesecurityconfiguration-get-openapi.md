---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API Describe Security Configuration
  version: 1.0.0
  description: Provides the details of a security configuration by returning the configuration
    JSON.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListSecurityConfigurations:
    get:
      summary: List Security Configurations
      description: Lists all the security configurations visible to this account,
        providing their creation dates and times, and their names.
      operationId: listSecurityConfigurations
      x-api-path-slug: actionlistsecurityconfigurations-get
      parameters:
      - in: query
        name: Marker
        description: The pagination token that indicates the set of results to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=CreateSecurityConfiguration:
    get:
      summary: Create Security Configuration
      description: Creates a security configuration, which is stored in the service
        and can be specified when a cluster is created.
      operationId: createSecurityConfiguration
      x-api-path-slug: actioncreatesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      - in: query
        name: SecurityConfiguration
        description: The security configuration details in JSON format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DeleteSecurityConfiguration:
    get:
      summary: Delete Security Configuration
      description: Deletes a security configuration.
      operationId: deleteSecurityConfiguration
      x-api-path-slug: actiondeletesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DescribeSecurityConfiguration:
    get:
      summary: Describe Security Configuration
      description: Provides the details of a security configuration by returning the
        configuration JSON.
      operationId: describeSecurityConfiguration
      x-api-path-slug: actiondescribesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
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