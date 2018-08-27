---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a VAT configuration by id
  description: Get a vat configuration by id.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/locations/revenue_account_configurations:
    get:
      summary: List revenue account configurations
      description: Lists revenue account configurations of a system. The revenue accounts
        are returned as paginated result. By default 50 revenue accounts are on one
        page.
      operationId: getRestAccountingLocationsRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationsrevenue-account-configurations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of revenue accounts to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Revenue
      - Account
      - Configurations
  /rest/vat:
    get:
      summary: List VAT configurations.
      description: Lists the VAT configurations for the given filter. Possible filters
        are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
        and <code>startedAt</code>.
      operationId: getRestVat
      x-api-path-slug: restvat-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: with
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
    post:
      summary: Create a VAT configuration
      description: Create a vat configuration.
      operationId: postRestVat
      x-api-path-slug: restvat-post
      parameters:
      - in: body
        name: /rest/vat
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
  /rest/vat/locations/{locationId}:
    get:
      summary: List VAT configurations of an accounting location
      description: Lists the VAT configurations for all countries of one accounting
        location
      operationId: getRestVatLocationsLocation
      x-api-path-slug: restvatlocationslocationid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/countries/{countryId}/revenue_accounts:
    get:
      summary: Get the revenue account configuration of a country
      description: Get the revenue account configuration of a country. The ID of the
        accounting location that the country is associated with as well as the ID
        of the country must be specified.
      operationId: getRestAccountingLocationsLocationCountriesCountryRevenueAccounts
      x-api-path-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
      parameters:
      - in: path
        name: countryId
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Country
  /rest/accounting/locations/{locationId}/debtor_account_configurations:
    get:
      summary: Get debtor account configuration of an accounting location
      description: Gets the debtor account configuration of an accounting location.
        The ID of the accounting location has to be specified. The debtor account
        configuration can contain one standard debtor account only or e.g. several
        accounts for each country of delivery.
      operationId: getRestAccountingLocationsLocationDebtorAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationiddebtor-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Debtor
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/posting_key_configurations:
    get:
      summary: Get a posting key configuration of an accounting location
      description: Gets a posting key configuration of an accounting location. The
        ID of the accounting location has to be specified. The posting key configuration
        can contain up to 4 posting keys.
      operationId: getRestAccountingLocationsLocationAddingKeyConfigurations
      x-api-path-slug: restaccountinglocationslocationidposting-key-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Key
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/revenue_account_configurations:
    get:
      summary: Get the revenue account configuration of an accounting location
      description: Gets the revenue account configuration of an accounting location.
        A revenue account location configuration contains several revenue accounts.
        The ID of the accounting location has to be specified.
      operationId: getRestAccountingLocationsLocationRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationidrevenue-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/item_sets/{setId}/config:
    get:
      summary: Get the item set configuration of an item set
      description: Get the item set configuration of an item set.
      operationId: getRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
      - Of
      - Item
      - Set
    put:
      summary: Update an item set configuration
      description: Update an item set configuration.
      operationId: putRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
  /rest/properties/groups/surcharge/types:
    get:
      summary: Get surcharge types from module configuration
      description: Get surcharge types from module configuration.
      operationId: getRestPropertiesGroupsSurchargeTypes
      x-api-path-slug: restpropertiesgroupssurchargetypes-get
      responses:
        200:
          description: OK
      tags:
      - Surcharge
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/types:
    get:
      summary: Get group types from module configuration
      description: Get group types from module configuration.
      operationId: getRestPropertiesGroupsTypes
      x-api-path-slug: restpropertiesgroupstypes-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Types
      - From
      - Module
      - Configuration
  /rest/vat/{vatId}:
    get:
      summary: Get a VAT configuration by id
      description: Get a vat configuration by id.
      operationId: getRestVatVat
      x-api-path-slug: restvatvatid-get
      parameters:
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
      - By
      - Id
    put:
      summary: Update a VAT configuration
      description: Update a vat configuration.
      operationId: putRestVatVat
      x-api-path-slug: restvatvatid-put
      parameters:
      - in: body
        name: /rest/vat/{vatId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
  /rest/vat/locations/{locationId}/countries/{countryId}/date/{date}:
    get:
      summary: Get a VAT configuration for a country in a location.
      description: Gets the VAT configuration found by matching the given location,
        delivery country and date of validity.
      operationId: getRestVatLocationsLocationCountriesCountryDateDate
      x-api-path-slug: restvatlocationslocationidcountriescountryiddatedate-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: date
      - in: path
        name: locationId
      - in: query
        name: startDate
        description: The date of validity
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationa
      - Country
      - In
      - Location
  /rest/vat/locations/{locationId}/countries/{countryId}:
    get:
      summary: List VAT configurations for one country of delivery
      description: Lists the VAT configurations for a country of delivery of one accounting
        location. The ID of the accounting location and the ID of the country of delivery
        must be specified.
      operationId: getRestVatLocationsLocationCountriesCountry
      x-api-path-slug: restvatlocationslocationidcountriescountryid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurationsone
      - Country
      - Of
      - Delivery
  /rest/logs/settings:
    get:
      summary: Show config.
      description: Show config..
      operationId: getRestLogsSettings
      x-api-path-slug: restlogssettings-get
      responses:
        200:
          description: OK
      tags:
      - Show
      - Config
    post:
      summary: Save config.
      description: Save config..
      operationId: postRestLogsSettings
      x-api-path-slug: restlogssettings-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Config
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