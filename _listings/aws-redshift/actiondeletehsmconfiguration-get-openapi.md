---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Delete Hsm Configuration
  version: 1.0.0
  description: Deletes the specified Amazon Redshift HSM configuration.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeHsmConfigurations:
    get:
      summary: Describe Hsm Configurations
      description: Returns information about the specified Amazon Redshift HSM configuration.
      operationId: describeHsmConfigurations
      x-api-path-slug: actiondescribehsmconfigurations-get
      parameters:
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier of a specific Amazon Redshift HSM configuration
          to be described
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          configurations that            are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM configurations            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=CreateHsmConfiguration:
    get:
      summary: Create Hsm Configuration
      description: |-
        Creates an HSM configuration that contains the information required by an Amazon Redshift
                    cluster to store and use database encryption keys in a Hardware Security Module (HSM).
      operationId: createHsmConfiguration
      x-api-path-slug: actioncreatehsmconfiguration-get
      parameters:
      - in: query
        name: Description
        description: A text description of the HSM configuration to be created
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier to be assigned to the new Amazon Redshift HSM
          configuration
        type: string
      - in: query
        name: HsmIpAddress
        description: The IP address that the Amazon Redshift cluster must use to access
          the HSM
        type: string
      - in: query
        name: HsmPartitionName
        description: The name of the partition in the HSM where the Amazon Redshift
          clusters will store their            database encryption keys
        type: string
      - in: query
        name: HsmPartitionPassword
        description: The password required to access the HSM partition
        type: string
      - in: query
        name: HsmServerPublicCertificate
        description: The HSMs public certificate file
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=DeleteHsmConfiguration:
    get:
      summary: Delete Hsm Configuration
      description: Deletes the specified Amazon Redshift HSM configuration.
      operationId: deleteHsmConfiguration
      x-api-path-slug: actiondeletehsmconfiguration-get
      parameters:
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier of the Amazon Redshift HSM configuration to be
          deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
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