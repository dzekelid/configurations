---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Configurations
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List revenue account configurations
  x-api-slug: restaccountinglocationsrevenue-account-configurations-get
  description: Lists revenue account configurations of a system. The revenue accounts
    are returned as paginated result. By default 50 revenue accounts are on one page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationsrevenue-account-configurations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationsrevenue-account-configurations-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations.
  x-api-slug: restvat-get
  description: Lists the VAT configurations for the given filter. Possible filters
    are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
    and <code>startedAt</code>.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvat-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations of an accounting location
  x-api-slug: restvatlocationslocationid-get
  description: Lists the VAT configurations for all countries of one accounting location
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationid-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of a country
  x-api-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
  description: Get the revenue account configuration of a country. The ID of the accounting
    location that the country is associated with as well as the ID of the country
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-openapi.md
- name: plentymarkets REST-API - Get debtor account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationiddebtor-account-configurations-get
  description: Gets the debtor account configuration of an accounting location. The
    ID of the accounting location has to be specified. The debtor account configuration
    can contain one standard debtor account only or e.g. several accounts for each
    country of delivery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationiddebtor-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get a posting key configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidposting-key-configurations-get
  description: Gets a posting key configuration of an accounting location. The ID
    of the accounting location has to be specified. The posting key configuration
    can contain up to 4 posting keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidposting-key-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidrevenue-account-configurations-get
  description: Gets the revenue account configuration of an accounting location. A
    revenue account location configuration contains several revenue accounts. The
    ID of the accounting location has to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidrevenue-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Get surcharge types from module configuration
  x-api-slug: restpropertiesgroupssurchargetypes-get
  description: Get surcharge types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-openapi.md
- name: plentymarkets REST-API - Get group types from module configuration
  x-api-slug: restpropertiesgroupstypes-get
  description: Get group types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-openapi.md
- name: plentymarkets REST-API - Create a VAT configuration
  x-api-slug: restvat-post
  description: Create a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvat-post-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration by id
  x-api-slug: restvatvatid-get
  description: Get a vat configuration by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-get-openapi.md
- name: plentymarkets REST-API - Update a VAT configuration
  x-api-slug: restvatvatid-put
  description: Update a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-put-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for a country in a location.
  x-api-slug: restvatlocationslocationidcountriescountryiddatedate-get
  description: Gets the VAT configuration found by matching the given location, delivery
    country and date of validity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryiddatedate-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations for one country of delivery
  x-api-slug: restvatlocationslocationidcountriescountryid-get
  description: Lists the VAT configurations for a country of delivery of one accounting
    location. The ID of the accounting location and the ID of the country of delivery
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryid-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of a country
  x-api-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
  description: Get the revenue account configuration of a country. The ID of the accounting
    location that the country is associated with as well as the ID of the country
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-openapi.md
- name: plentymarkets REST-API - Get debtor account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationiddebtor-account-configurations-get
  description: Gets the debtor account configuration of an accounting location. The
    ID of the accounting location has to be specified. The debtor account configuration
    can contain one standard debtor account only or e.g. several accounts for each
    country of delivery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationiddebtor-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get a posting key configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidposting-key-configurations-get
  description: Gets a posting key configuration of an accounting location. The ID
    of the accounting location has to be specified. The posting key configuration
    can contain up to 4 posting keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidposting-key-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidrevenue-account-configurations-get
  description: Gets the revenue account configuration of an accounting location. A
    revenue account location configuration contains several revenue accounts. The
    ID of the accounting location has to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidrevenue-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Get surcharge types from module configuration
  x-api-slug: restpropertiesgroupssurchargetypes-get
  description: Get surcharge types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-openapi.md
- name: plentymarkets REST-API - Get group types from module configuration
  x-api-slug: restpropertiesgroupstypes-get
  description: Get group types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-openapi.md
- name: plentymarkets REST-API - Create a VAT configuration
  x-api-slug: restvat-post
  description: Create a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvat-post-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration by id
  x-api-slug: restvatvatid-get
  description: Get a vat configuration by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-get-openapi.md
- name: plentymarkets REST-API - Update a VAT configuration
  x-api-slug: restvatvatid-put
  description: Update a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-put-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for a country in a location.
  x-api-slug: restvatlocationslocationidcountriescountryiddatedate-get
  description: Gets the VAT configuration found by matching the given location, delivery
    country and date of validity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryiddatedate-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations for one country of delivery
  x-api-slug: restvatlocationslocationidcountriescountryid-get
  description: Lists the VAT configurations for a country of delivery of one accounting
    location. The ID of the accounting location and the ID of the country of delivery
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryid-get-openapi.md
- name: plentymarkets REST-API - Show config.
  x-api-slug: restlogssettings-get
  description: Show config..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-get-openapi.md
- name: plentymarkets REST-API - Save config.
  x-api-slug: restlogssettings-post
  description: Save config..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-post-openapi.md
- name: plentymarkets REST-API - Save config.
  x-api-slug: restlogssettings-post
  description: Save config..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-post-openapi.md
- name: plentymarkets REST-API - Show config.
  x-api-slug: restlogssettings-get
  description: Show config..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restlogssettings-get-openapi.md
- name: plentymarkets REST-API - Update a VAT configuration
  x-api-slug: restvatvatid-put
  description: Update a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-put-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration by id
  x-api-slug: restvatvatid-get
  description: Get a vat configuration by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatvatid-get-openapi.md
- name: plentymarkets REST-API - Create a VAT configuration
  x-api-slug: restvat-post
  description: Create a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvat-post-openapi.md
- name: plentymarkets REST-API - Get group types from module configuration
  x-api-slug: restpropertiesgroupstypes-get
  description: Get group types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupstypes-get-openapi.md
- name: plentymarkets REST-API - Get surcharge types from module configuration
  x-api-slug: restpropertiesgroupssurchargetypes-get
  description: Get surcharge types from module configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restpropertiesgroupssurchargetypes-get-openapi.md
- name: plentymarkets REST-API - Update an item set configuration
  x-api-slug: restitem-setssetidconfig-put
  description: Update an item set configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-put-openapi.md
- name: plentymarkets REST-API - Get the item set configuration of an item set
  x-api-slug: restitem-setssetidconfig-get
  description: Get the item set configuration of an item set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restitem-setssetidconfig-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidrevenue-account-configurations-get
  description: Gets the revenue account configuration of an accounting location. A
    revenue account location configuration contains several revenue accounts. The
    ID of the accounting location has to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidrevenue-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get a posting key configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidposting-key-configurations-get
  description: Gets a posting key configuration of an accounting location. The ID
    of the accounting location has to be specified. The posting key configuration
    can contain up to 4 posting keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidposting-key-configurations-get-openapi.md
- name: plentymarkets REST-API - Get debtor account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationiddebtor-account-configurations-get
  description: Gets the debtor account configuration of an accounting location. The
    ID of the accounting location has to be specified. The debtor account configuration
    can contain one standard debtor account only or e.g. several accounts for each
    country of delivery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationiddebtor-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of a country
  x-api-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
  description: Get the revenue account configuration of a country. The ID of the accounting
    location that the country is associated with as well as the ID of the country
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restaccountinglocationslocationidcountriescountryidrevenue-accounts-get-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for a country in a location.
  x-api-slug: restvatlocationslocationidcountriescountryiddatedate-get
  description: Gets the VAT configuration found by matching the given location, delivery
    country and date of validity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryiddatedate-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations for one country of delivery
  x-api-slug: restvatlocationslocationidcountriescountryid-get
  description: Lists the VAT configurations for a country of delivery of one accounting
    location. The ID of the accounting location and the ID of the country of delivery
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/configurations/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryid-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---