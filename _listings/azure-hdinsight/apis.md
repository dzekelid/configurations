---
name: Azure HDInsight
x-slug: azure-hdinsight
description: Azure HDInsight is a Hadoop-based service that brings an Apache Hadoop
  solution to the cloud. Gain the full value of big data with a cloud-based data platform
  that manages data of any type and size.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-hdinsights-open-source-analytics.png
x-kinRank: "10"
x-alexaRank: ""
tags: Configurations
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/azure-hdinsight/apis.md
specificationVersion: "0.14"
apis:
- name: Azure HDInsight API Configurations Update HTTPSettings
  x-api-slug: azure-hdinsight-api
  description: Begins configuring the HTTP settings on the specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-hdinsights-open-source-analytics.png
  humanURL: https://azure.microsoft.com/en-us/services/hdinsight/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/configurations/{configurationName}
  tags: Configurations Httpsettings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/azure-hdinsight/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-post-openapi.md
- name: Azure HDInsight API Configurations Get
  x-api-slug: azure-hdinsight-api
  description: The configuration object for the specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-hdinsights-open-source-analytics.png
  humanURL: https://azure.microsoft.com/en-us/services/hdinsight/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/configurations/{configurationName}
  tags: Configurations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/azure-hdinsight/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/azure-hdinsight/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-get-openapi.md
- name: Azure HDInsight API
  x-api-slug: azure-hdinsight-api
  description: Azure HDInsight is a Hadoop-based service that brings an Apache Hadoop
    solution to the cloud. Gain the full value of big data with a cloud-based data
    platform that manages data of any type and size.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-hdinsights-open-source-analytics.png
  humanURL: https://azure.microsoft.com/en-us/services/hdinsight/
  baseURL: ://management.azure.com//
  tags: Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/azure-hdinsight/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/hdinsight/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/hdinsight/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/hdinsight/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/hdinsight/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---