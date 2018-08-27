swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /config:
    get:
      summary: Get configuration
      description: |-
        Retrieve the current server configuration
        ##### Permissions
        Must have `manage_system` permission.
      operationId: retrieve-the-current-server-configuration-permissionsmust-have-manage-system-permission
      x-api-path-slug: config-get
      responses:
        200:
          description: OK
      tags:
      - Configuration
    put:
      summary: Update configuration
      description: |-
        Submit a new configuration for the server to use. As of server version 4.8, the `PluginSettings.EnableUploads` setting cannot be modified by this endpoint.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: submit-a-new-configuration-for-the-server-to-use-as-of-server-version-48-the-pluginsettingsenableupl
      x-api-path-slug: config-put
      parameters:
      - in: body
        name: body
        description: Mattermost configuration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Configuration
  /config/reload:
    post:
      summary: Reload configuration
      description: |-
        Reload the configuration file to pick up on any changes made to it.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: reload-the-configuration-file-to-pick-up-on-any-changes-made-to-it-permissionsmust-have-manage-syste
      x-api-path-slug: configreload-post
      responses:
        200:
          description: OK
      tags:
      - Reload
      - Configuration
  /config/client:
    get:
      summary: Get client configuration
      description: |-
        Get a subset of the server configuration needed by the client.
        ##### Permissions
        No permission required.
      operationId: get-a-subset-of-the-server-configuration-needed-by-the-client-permissionsno-permission-required
      x-api-path-slug: configclient-get
      parameters:
      - in: query
        name: format
        description: Must be `old`, other formats not implemented yet
      responses:
        200:
          description: OK
      tags:
      - Client
      - Configuration
  /config/environment:
    get:
      summary: Get configuration made through environment variables
      description: |-
        Retrieve a json object mirroring the server configuration where fields are set to true
        if the corresponding config setting is set through an environment variable. Settings
        that haven't been set through environment variables will be missing from the object.

        __Minimum server version__: 4.10

        ##### Permissions
        Must have `manage_system` permission.
      operationId: retrieve-a-json-object-mirroring-the-server-configuration-where-fields-are-set-to-trueif-the-corresp
      x-api-path-slug: configenvironment-get
      responses:
        200:
          description: OK
      tags:
      - Configuration
      - Made
      - Through
      - Environment
      - Variables
  /ldap/test:
    post:
      summary: Test LDAP configuration
      description: |-
        Test the current AD/LDAP configuration to see if the AD/LDAP server can be contacted successfully.
        ##### Permissions
        Must have `manage_system` permission.
      operationId: test-the-current-adldap-configuration-to-see-if-the-adldap-server-can-be-contacted-successfully-perm
      x-api-path-slug: ldaptest-post
      responses:
        200:
          description: OK
      tags:
      - Test
      - LDAP
      - Configuration
  /elasticsearch/test:
    post:
      summary: Test Elasticsearch configuration
      description: |-
        Test the current Elasticsearch configuration to see if the Elasticsearch server can be contacted successfully.
        Optionally provide a configuration in the request body to test. If no valid configuration is present in the
        request body the current server configuration will be tested.

        __Minimum server version__: 4.1
        ##### Permissions
        Must have `manage_system` permission.
      operationId: test-the-current-elasticsearch-configuration-to-see-if-the-elasticsearch-server-can-be-contacted-suc
      x-api-path-slug: elasticsearchtest-post
      responses:
        200:
          description: OK
      tags:
      - Test
      - Elasticsearch
      - Configuration