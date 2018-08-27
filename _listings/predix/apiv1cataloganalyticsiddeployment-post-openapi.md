---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Framework Deploy an analytic with an optional deployment
    configuration by analytic catalog entry id.
  version: 1.0.0
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment with an optional deployment configuration, responds with the
    request id (generated for the request), and the current request status.  The force
    deploy usually takes longer than the standard timeout, so the calling process
    should use the returned request id to monitor the request status and to retrieve
    the deployment results.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/connector/resource:
    get:
      summary: Retrieves connector configuration for external resource attributes
        for the given zone.
      description: Retrieves connector configuration for external resource attributes
        for the given zone..
      operationId: getResourceConnectorUsingGET_1
      x-api-path-slug: v1connectorresource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external resource attributes
        for the given zone.
      description: Creates or updates connector configuration for external resource
        attributes for the given zone..
      operationId: putResourceConnectorUsingPUT_1
      x-api-path-slug: v1connectorresource-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external resource
          attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external resource attributes for
        the given zone.
      description: Deletes connector configuration for external resource attributes
        for the given zone..
      operationId: deleteResourceConnectorUsingDELETE
      x-api-path-slug: v1connectorresource-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
  /v1/connector/subject:
    get:
      summary: Retrieves connector configuration for external subject attributes for
        the given zone.
      description: Retrieves connector configuration for external subject attributes
        for the given zone..
      operationId: getSubjectConnectorUsingGET
      x-api-path-slug: v1connectorsubject-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external subject attributes
        for the given zone.
      description: Creates or updates connector configuration for external subject
        attributes for the given zone..
      operationId: putSubjectConnectorUsingPUT_1
      x-api-path-slug: v1connectorsubject-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external subject attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external subject attributes for
        the given zone.
      description: Deletes connector configuration for external subject attributes
        for the given zone..
      operationId: deleteSubjectConnectorUsingDELETE
      x-api-path-slug: v1connectorsubject-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
  /api/v1/catalog/analytics/{id}/deployment:
    post:
      summary: Deploy an analytic with an optional deployment configuration by analytic
        catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment with an optional deployment configuration, responds with
        the request id (generated for the request), and the current request status.  The
        force deploy usually takes longer than the standard timeout, so the calling
        process should use the returned request id to monitor the request status and
        to retrieve the deployment results.
      operationId: deployAnalytic
      x-api-path-slug: apiv1cataloganalyticsiddeployment-post
      parameters:
      - in: body
        name: body
        description: deployment configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Deploy
      - Analytic
      - Optional
      - Deployment
      - Configuration
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v2/config/orchestrations:
    get:
      summary: Get all orchestration configuration entries.
      description: Returns all orchestration configuration entries as specified by
        page and sort criteria.
      operationId: retrieveAllOrchConfigs
      x-api-path-slug: apiv2configorchestrations-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      responses:
        2:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entries
    post:
      summary: Create an orchestration configuration entry.
      description: Creates the orchestration configuration entry with a generated
        id.
      operationId: createOrchestrationEntry
      x-api-path-slug: apiv2configorchestrations-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/artifacts:
    post:
      summary: Upload an artifact and attach it to an orchestration configuration
        entry.
      description: Upload a single artifact file in a multipart MIME structure and
        attach it to an orchestration configuration entry. The multipart MIME structure
        must have the orchestration entry id tagged as 'orchestrationEntryId',  the
        file contents tagged as 'file',  the artifact type tagged as 'type', and  the
        name of artifact tagged as 'name'.  A description (under 1024 characters)
        tagged as 'description' can be optionally specified. Artifact types can be
        either 'portToFieldMap', 'bpmn' or any.   If the artifact type is 'portToFieldMap',
        specify the orchestration step ID tagged as 'stepId'.   Otherwise, 'name'
        will be used as 'stepId'.  (See the documentation for more information regarding
        these files.)
      operationId: uploadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifacts-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: (Required) Artifact file
      - in: formData
        name: name
        description: (Required) Artifact name
      - in: formData
        name: orchestrationEntryId
        description: (Required) orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: formData
        name: stepId
        description: Orchestration Step ID
      - in: formData
        name: type
        description: (Required) Artifact type
      responses:
        2:
          description: Successful response
      tags:
      - Upload
      - Artifact
      - Attach
      - It
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/{id}:
    get:
      summary: Get an orchestration configuration entry by id.
      description: Returns the orchestration configuration entry with the given id.
      operationId: retrieveOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
    put:
      summary: Update an existing orchestration configuration entry.
      description: Updates the orchestration configuration entry with given orchestration
        configuration.
      operationId: updateOrchestrationEntry
      x-api-path-slug: apiv2configorchestrationsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: orchestration configuration id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Existing
      - Orchestration
      - Configuration
      - Entry
    delete:
      summary: Delete an orchestration configuration entry by id.
      description: Deletes the orchestration configuration entry with the given id.
      operationId: deleteOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
  /api/v2/config/orchestrations/{id}/artifacts:
    get:
      summary: Get the descriptive information of the orchestration artifacts corresponding
        to an orchestration configuration entry.
      description: 'Returns the description information (type, description, etc.)
        for all orchestration artifacts associated with the given configuration entry
        id. Note: it does not return the orchestration artifact file contents; use
        the download APIs to obtain an artifact file. An error is returned if the
        supplied orchestration configuration entry id does not exist.'
      operationId: retrieveArtifactsByOrchestrationEntryId
      x-api-path-slug: apiv2configorchestrationsidartifacts-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Descriptive
      - Information
      - Of
      - Orchestration
      - Artifacts
      - Corresponding
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/execution/orchestrations/{orchConfigId}/deployment:
    post:
      summary: Deploy the specified orchestration workflow file to the Orchestration
        Engine.
      description: This API will deploy the BPMN file associated with the specified
        orchestration configuration to the Orchestration Engine in preparation for
        orchestration execution.
      operationId: retrieveAndDeployBpmn
      x-api-path-slug: apiv2executionorchestrationsorchconfigiddeployment-post
      parameters:
      - in: path
        name: orchConfigId
        description: orchestration configuration id
      responses:
        2:
          description: Successful response
      tags:
      - Deploy
      - Specified
      - Orchestration
      - Workflow
      - File
      - To
      - Orchestration
      - Engine
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