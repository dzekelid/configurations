---
swagger: "2.0"
x-collection-name: Azure HDInsight
x-complete: 0
info:
  title: Azure HDInsight API Configurations Update HTTPSettings
  description: Begins configuring the HTTP settings on the specified cluster.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/configurations/{configurationName}
  : post:
      summary: Configurations Update HTTPSettings
      description: Begins configuring the HTTP settings on the specified cluster.
      operationId: Configurations_UpdateHTTPSettings
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-hdinsightclustersclusternameconfigurationsconfigurationname-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: configurationName
        description: The constant for configuration type of gateway
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The name of the resource group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Configurations Httpsettings
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