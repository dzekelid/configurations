swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/users/{userId}/managedConfigurationsForUser:
    get:
      summary: Get Per User Configurations
      description: Lists all the per-user managed configurations for the specified
        user. Only the ID is set.
      operationId: androidenterprise.managedconfigurationsforuser.list
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforuser-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
  /enterprises/{enterpriseId}/users/{userId}/managedConfigurationsForUser/{managedConfigurationForUserId}:
    delete:
      summary: Delete Per User Configurations
      description: Removes a per-user managed configuration for an app for the specified
        user.
      operationId: androidenterprise.managedconfigurationsforuser.delete
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    get:
      summary: Get Per User Configuration
      description: Retrieves details of a per-user managed configuration for an app
        for the specified user.
      operationId: androidenterprise.managedconfigurationsforuser.get
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    patch:
      summary: Update Per User Configuration
      description: Adds or updates a per-user managed configuration for an app for
        the specified user. This method supports patch semantics.
      operationId: androidenterprise.managedconfigurationsforuser.patch
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    put:
      summary: Update Per User Configuration
      description: Adds or updates a per-user managed configuration for an app for
        the specified user.
      operationId: androidenterprise.managedconfigurationsforuser.update
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration