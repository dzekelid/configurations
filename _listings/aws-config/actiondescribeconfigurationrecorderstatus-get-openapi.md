---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Describe Configuration Recorder Status
  version: 1.0.0
  description: Returns the current status of the specified configuration recorder.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteConfigurationRecorder:
    get:
      summary: Delete Configuration Recorder
      description: Deletes the configuration recorder.
      operationId: deleteConfigurationRecorder
      x-api-path-slug: actiondeleteconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the configuration recorder to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=DescribeConfigurationRecorders:
    get:
      summary: Describe Configuration Recorders
      description: Returns the details for the specified configuration recorders.
      operationId: describeConfigurationRecorders
      x-api-path-slug: actiondescribeconfigurationrecorders-get
      parameters:
      - in: query
        name: ConfigurationRecorderNames
        description: A list of configuration recorder names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DescribeConfigurationRecorderStatus:
    get:
      summary: Describe Configuration Recorder Status
      description: Returns the current status of the specified configuration recorder.
      operationId: describeConfigurationRecorderStatus
      x-api-path-slug: actiondescribeconfigurationrecorderstatus-get
      parameters:
      - in: query
        name: ConfigurationRecorderNames
        description: The name(s) of the configuration recorder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=PutConfigurationRecorder:
    get:
      summary: Put Configuration Recorder
      description: Creates a new configuration recorder to record the selected resource
        configurations.
      operationId: putConfigurationRecorder
      x-api-path-slug: actionputconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorder
        description: The configuration recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=StartConfigurationRecorder:
    get:
      summary: Start Configuration Recorder
      description: Starts recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: startConfigurationRecorder
      x-api-path-slug: actionstartconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=StopConfigurationRecorder:
    get:
      summary: Stop Configuration Recorder
      description: Stops recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: stopConfigurationRecorder
      x-api-path-slug: actionstopconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=DeleteConfigRule:
    get:
      summary: Delete Config Rule
      description: Deletes the specified AWS Config rule and all of its evaluation
        results.
      operationId: deleteConfigRule
      x-api-path-slug: actiondeleteconfigrule-get
      parameters:
      - in: query
        name: ConfigRuleName
        description: The name of the AWS Config rule that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DeleteEvaluationResults:
    get:
      summary: Delete Evaluation Results
      description: Deletes the evaluation results for the specified Config rule.
      operationId: deleteEvaluationResults
      x-api-path-slug: actiondeleteevaluationresults-get
      parameters:
      - in: query
        name: ConfigRuleName
        description: The name of the Config rule for which you want to delete the
          evaluation results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=DeliverConfigSnapshot:
    get:
      summary: Deliver Config Snapshot
      description: Schedules delivery of a configuration snapshot to the Amazon S3
        bucket in the specified delivery channel.
      operationId: deliverConfigSnapshot
      x-api-path-slug: actiondeliverconfigsnapshot-get
      parameters:
      - in: query
        name: deliveryChannelName
        description: The name of the delivery channel through which the snapshot is
          delivered
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Snapshot
  /?Action=DescribeComplianceByConfigRule:
    get:
      summary: Describe Compliance By Config Rule
      description: Indicates whether the specified AWS Config rules are compliant.
      operationId: describeComplianceByConfigRule
      x-api-path-slug: actiondescribecompliancebyconfigrule-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: ConfigRuleNames
        description: Specify one or more AWS Config rule names to filter the results
          by rule
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=DescribeConfigRuleEvaluationStatus:
    get:
      summary: Describe Config Rule Evaluation Status
      description: Returns status information for each of your AWS managed Config
        rules.
      operationId: describeConfigRuleEvaluationStatus
      x-api-path-slug: actiondescribeconfigruleevaluationstatus-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The name of the AWS managed Config rules for which you want status
          information
        type: string
      - in: query
        name: Limit
        description: The number of rule evaluation results that you want returned
        type: string
      - in: query
        name: NextToken
        description: The NextToken string returned on a previous page that you use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=DescribeConfigRules:
    get:
      summary: Describe Config Rules
      description: Returns details about your AWS Config rules.
      operationId: describeConfigRules
      x-api-path-slug: actiondescribeconfigrules-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The names of the AWS Config rules for which you want details
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
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