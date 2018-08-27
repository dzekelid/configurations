swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 1
info:
  title: AutomationManagementClient
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/configurations/{configurationName}
  : delete:
      summary: Dsc Configuration Delete
      description: Delete the dsc configuration identified by configuration name.
      operationId: DscConfiguration_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameconfigurationsconfigurationname-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: configurationName
        description: The configuration name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Configuration
    get:
      summary: Dsc Configuration Get
      description: Retrieve the configuration identified by configuration name.
      operationId: DscConfiguration_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameconfigurationsconfigurationname-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: configurationName
        description: The configuration name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Configuration
    put:
      summary: Dsc Configuration Create Or Update
      description: Create the configuration identified by configuration name.
      operationId: DscConfiguration_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameconfigurationsconfigurationname-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: configurationName
        description: The create or update parameters for configuration
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The create or update parameters for configuration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Configuration
      - Or
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/configurations/{configurationName}/content
  : get:
      summary: Dsc Configuration Get Content
      description: Retrieve the configuration script identified by configuration name.
      operationId: DscConfiguration_GetContent
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameconfigurationsconfigurationnamecontent-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: configurationName
        description: The configuration name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Configuration
      - ""
      - Content
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/configurations
  : get:
      summary: Dsc Configuration List By Automation Account
      description: Retrieve a list of configurations.
      operationId: DscConfiguration_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnameconfigurations-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Configuration
      - List
      - Automation
      - Account
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/nodeConfigurations/{nodeConfigurationName}
  : delete:
      summary: Dsc Node Configuration Delete
      description: Delete the Dsc node configurations by node configuration.
      operationId: DscNodeConfiguration_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodeconfigurationsnodeconfigurationname-delete
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: nodeConfigurationName
        description: The Dsc node configuration name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Node
      - Configuration
    get:
      summary: Dsc Node Configuration Get
      description: Retrieve the Dsc node configurations by node configuration.
      operationId: DscNodeConfiguration_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodeconfigurationsnodeconfigurationname-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: nodeConfigurationName
        description: The Dsc node configuration name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Node
      - Configuration
    put:
      summary: Dsc Node Configuration Create Or Update
      description: Create the node configuration identified by node configuration
        name.
      operationId: DscNodeConfiguration_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodeconfigurationsnodeconfigurationname-put
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      - in: path
        name: nodeConfigurationName
        description: The create or update parameters for configuration
      - in: body
        name: parameters
        description: The create or update parameters for configuration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Node
      - Configuration
      - Or
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/nodeConfigurations
  : get:
      summary: Dsc Node Configuration List By Automation Account
      description: Retrieve a list of dsc node configurations.
      operationId: DscNodeConfiguration_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamenodeconfigurations-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Dsc
      - Node
      - Configuration
      - List
      - Automation
      - Account