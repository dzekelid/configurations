---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API List Deployment Configs
  version: 1.0.0
  description: |-
    Lists the deployment configurations with the applicable IAM user or AWS
                account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDeploymentConfig:
    get:
      summary: Create Deployment Config
      description: Creates a deployment configuration.
      operationId: createDeploymentConfig
      x-api-path-slug: actioncreatedeploymentconfig-get
      parameters:
      - in: query
        name: deploymentConfigName
        description: The name of the deployment configuration to create
        type: string
      - in: query
        name: minimumHealthyHosts
        description: The minimum number of healthy instances that should be available
          at any time during            the deployment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=DeleteDeploymentConfig:
    get:
      summary: Delete Deployment Config
      description: Deletes a deployment configuration.
      operationId: deleteDeploymentConfig
      x-api-path-slug: actiondeletedeploymentconfig-get
      parameters:
      - in: query
        name: deploymentConfigName
        description: The name of a deployment configuration associated with the applicable
          IAM user or            AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=GetDeploymentConfig:
    get:
      summary: Get Deployment Config
      description: Gets information about a deployment configuration.
      operationId: getDeploymentConfig
      x-api-path-slug: actiongetdeploymentconfig-get
      parameters:
      - in: query
        name: deploymentConfigName
        description: The name of a deployment configuration associated with the applicable
          IAM user or            AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
  /?Action=ListDeploymentConfigs:
    get:
      summary: List Deployment Configs
      description: |-
        Lists the deployment configurations with the applicable IAM user or AWS
                    account.
      operationId: listDeploymentConfigs
      x-api-path-slug: actionlistdeploymentconfigs-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment configurations
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployments
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