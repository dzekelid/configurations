---
swagger: "2.0"
x-collection-name: Azure HDInsight
x-complete: 1
info:
  title: HDInsightManagementClient
  description: the-hdinsight-management-client
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-post
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
    get:
      summary: Configurations Get
      description: The configuration object for the specified cluster.
      operationId: Configurations_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: configurationName
        description: The constant for configuration type of gateway
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Configurations
---