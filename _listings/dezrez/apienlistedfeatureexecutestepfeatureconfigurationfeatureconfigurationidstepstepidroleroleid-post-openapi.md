---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: 'Dezrez '
  version: 1.0.0
  description: .
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/role/{id}/setportaloverrides:
    put:
      summary: Set portal configuration exclusivity overrides
      description: Set portal configuration exclusivity overrides.
      operationId: Role_SetPortalConfigurationDelayOverridesByidBydatacontract
      x-api-path-slug: apiroleidsetportaloverrides-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Portal
      - Configuration
      - Exclusivity
      - Overrides
  /api/agency/milestoneconfigurations:
    get:
      summary: Get the milestone configurations for an agency
      description: Get the milestone configurations for an agency.
      operationId: Agency_MilestoneConfigurations
      x-api-path-slug: apiagencymilestoneconfigurations-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Milestone
      - Configurationsan
      - Agency
  /api/agency/portalconfigurations:
    get:
      summary: Get a list of portal configurations for the brand within a branch.
      description: Get a list of portal configurations for the brand within a branch..
      operationId: Agency_PortalConfigurationsBypageSizeBypageNumber
      x-api-path-slug: apiagencyportalconfigurations-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Portal
      - Configurationsthe
      - Brand
      - Within
      - Branch
  /api/enlistedfeature/executestep/featureConfiguration/{featureConfigurationId}/step/{stepId}/role/{roleId}:
    post:
      summary: ""
      description: .
      operationId: EnlistedFeature_ExecuteStepByroleIdByfeatureConfigurationIdBystepIdByinvocationDataContractBychosenE
      x-api-path-slug: apienlistedfeatureexecutestepfeatureconfigurationfeatureconfigurationidstepstepidroleroleid-post
      parameters:
      - in: query
        name: chosenExternalProviderId
      - in: path
        name: featureConfigurationId
      - in: body
        name: invocationDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      - in: path
        name: stepId
      responses:
        200:
          description: OK
      tags:
      - ""
  /api/screenz/config/{screenid}:
    get:
      summary: Gets the config back for a screen with a guid that was registered against
        a branch
      description: Gets the config back for a screen with a guid that was registered
        against a branch.
      operationId: Screenz_ConfigByscreenid
      x-api-path-slug: apiscreenzconfigscreenid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: screenid
      responses:
        200:
          description: OK
      tags:
      - S
      - Config
      - Backa
      - Screen
      - Guid
      - That
      - Was
      - Registered
      - Against
      - Branch
  /api/screenz/registered:
    get:
      summary: Gets the config back for a screen with a guid that was registered against
        a branch
      description: Gets the config back for a screen with a guid that was registered
        against a branch.
      operationId: Screenz_Registered
      x-api-path-slug: apiscreenzregistered-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Config
      - Backa
      - Screen
      - Guid
      - That
      - Was
      - Registered
      - Against
      - Branch
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