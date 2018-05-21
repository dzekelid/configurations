---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API Get a Domain
  description: Get a Domain
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /etp-report/v1/configs/{configId}/threat-events/aggregate:
    get:
      summary: Report Security Event Aggregation
      description: Report Security Event Aggregation
      operationId: etpreportv1configsconfigidthreateventsaggregatestarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigidthreateventsaggregate-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - Threat
      - Events
      - Aggregation
      - Starttimesec
      - endtimesec
      - dimension
      - filters
      - Aggregation
  /etp-report/v1/configs/{configId}/threat-events/details:
    get:
      summary: Report Security Event Details
      description: Report Security Event Details
      operationId: etpreportv1configsconfigidthreateventsdetailsstarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigidthreateventsdetails-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - Threat
      - Events
      - Details
      - Starttimesec
      - endtimesec
      - dimension
      - filters
  /etp-report/v1/configs/{configId}/threat-events/time-series:
    get:
      summary: Report Security Event Time Series
      description: Report Security Event Time Series
      operationId: etpreportv1configsconfigidthreateventstimeseriesstarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigidthreateventstimeseries-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - Threat
      - Events
      - Time
      - Series
      - Starttimesec
      - endtimesec
      - dimension
      - filters
  /etp-report/v1/configs/{configId}/aup-events/details:
    get:
      summary: Report AUP Event Details
      description: Report AUP Event Details
      operationId: etpreportv1configsconfigidaupeventsdetailsstarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigidaupeventsdetails-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - Aup
      - Events
      - Details
      - Starttimesec
      - endtimesec
      - dimension
      - filters
  /etp-report/v1/configs/{configId}/aup-events/time-series:
    get:
      summary: Report AUP Event Time Series
      description: Report AUP Event Time Series
      operationId: etpreportv1configsconfigidaupeventstimeseriesstarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigidaupeventstimeseries-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - Aup
      - Events
      - Time
      - Series
      - Starttimesec
      - endtimesec
      - dimension
      - filters
  /etp-report/v1/configs/{configId}/dns-activities/time-series:
    get:
      summary: Report DNS Activity Time Series
      description: Report DNS Activity Time Series
      operationId: etpreportv1configsconfigiddnsactivitiestimeseriesstarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigiddnsactivitiestimeseries-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - DNS
      - Activities
      - Time
      - Series
      - Starttimesec
      - endtimesec
      - dimension
      - filters
  /etp-report/v1/configs/{configId}/dns-activities/aggregate:
    get:
      summary: Report DNS Activities Totals
      description: Report DNS Activities Totals
      operationId: etpreportv1configsconfigiddnsactivitiesaggregatestarttimesecendtimesecdimensionfilters
      x-api-path-slug: etpreportv1configsconfigiddnsactivitiesaggregate-get
      parameters:
      - in: query
        name: configId
        description: ETP Configuration identifier assigned to the customer
        type: string
      - in: query
        name: dimension
        description: Flag to group the data
        type: string
      - in: query
        name: endTimeSec
        description: Timestamp for the end of the data window, in UTC seconds format
        type: string
      - in: query
        name: filters
        description: filter parameters to filter the data
        type: string
      - in: query
        name: startTimeSec
        description: Timestamp for the start of the data window, in UTC seconds format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Etp
      - Report
      - Configurationss
      - Configurations
      - DNS
      - Activities
      - Aggregation
      - Starttimesec
      - endtimesec
      - dimension
      - filters
      - Aggregation
  acgObject:
    get:
      summary: List Configurations
      description: List Configurations
      operationId: acgobject
      x-api-path-slug: acgobject-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
  /lds/v1/configurations/resume/{serviceId}:
    post:
      summary: Resume a Configuration
      description: Resume a Configuration
      operationId: ldsv1configurationsresumeserviceid
      x-api-path-slug: ldsv1configurationsresumeserviceid-post
      parameters:
      - in: query
        name: serviceId
        description: ID of the configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Lds
      - Configurationsurations
      - Resume
      - Service
  /config-media-live/v1/live:
    get:
      summary: List Domains
      description: List Domains
      operationId: configmedialivev1live
      x-api-path-slug: configmedialivev1live-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
    post:
      summary: Create a Domain
      description: Create a Domain
      operationId: configmedialivev1live
      x-api-path-slug: configmedialivev1live-post
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
  /config-media-live/v1/live/{domain}:
    get:
      summary: Get a Domain
      description: Get a Domain
      operationId: configmedialivev1livedomain
      x-api-path-slug: configmedialivev1livedomain-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
    delete:
      summary: Remove a Domain
      description: Remove a Domain
      operationId: configmedialivev1livedomain
      x-api-path-slug: configmedialivev1livedomain-delete
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
  /config-media-live/v1/live/{domain}/stream:
    get:
      summary: List Streams
      description: List Streams
      operationId: configmedialivev1livedomainstream
      x-api-path-slug: configmedialivev1livedomainstream-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
    post:
      summary: Create a New Stream
      description: Create a New Stream
      operationId: configmedialivev1livedomainstream
      x-api-path-slug: configmedialivev1livedomainstream-post
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
  /config-media-live/v1/live/{domain}/stream/{streamId}:
    get:
      summary: Get a Stream
      description: Get a Stream
      operationId: configmedialivev1livedomainstreamstreamid
      x-api-path-slug: configmedialivev1livedomainstreamstreamid-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
    delete:
      summary: Remove a Stream
      description: Remove a Stream
      operationId: configmedialivev1livedomainstreamstreamid
      x-api-path-slug: configmedialivev1livedomainstreamstreamid-delete
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
    put:
      summary: Modify a Stream
      description: Modify a Stream
      operationId: configmedialivev1livedomainstreamstreamid
      x-api-path-slug: configmedialivev1livedomainstreamstreamid-put
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
  /config-media-live/v1/live/{domain}/stream/{streamId}/event:
    get:
      summary: List Events
      description: List Events
      operationId: configmedialivev1livedomainstreamstreamidevent
      x-api-path-slug: configmedialivev1livedomainstreamstreamidevent-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
      - Event
  /config-media-live/v1/live/{domain}/stream/{streamId}/event/{eventName}:
    get:
      summary: Get an Event
      description: Get an Event
      operationId: configmedialivev1livedomainstreamstreamideventeventname
      x-api-path-slug: configmedialivev1livedomainstreamstreamideventeventname-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: eventName
        description: Human-readable event name
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
      - Event
      - Eventname
    put:
      summary: Modify an Event
      description: Modify an Event
      operationId: configmedialivev1livedomainstreamstreamideventeventname
      x-api-path-slug: configmedialivev1livedomainstreamstreamideventeventname-put
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: eventName
        description: Human-readable event name
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
      - Event
      - Eventname
    delete:
      summary: Remove an Event
      description: Remove an Event
      operationId: configmedialivev1livedomainstreamstreamideventeventname
      x-api-path-slug: configmedialivev1livedomainstreamstreamideventeventname-delete
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: eventName
        description: Human-readable event name
        type: string
      - in: query
        name: streamId
        description: Unique identifier for each stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Stream
      - Stream
      - Event
      - Eventname
  /config-media-live/v1/live/{domain}/version:
    post:
      summary: Create a New Version
      description: Create a New Version
      operationId: configmedialivev1livedomainversion
      x-api-path-slug: configmedialivev1livedomainversion-post
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Version
  /config-media-live/v1/live/{domain}/version/{versionId}:
    get:
      summary: Get a Version
      description: Get a Version
      operationId: configmedialivev1livedomainversionversionid
      x-api-path-slug: configmedialivev1livedomainversionversionid-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: versionId
        description: Domain&#8217;s incremental version number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Version
  /config-media-live/v1/live/{domain}/version/{versionId}/activation:
    get:
      summary: Get Activation Status
      description: Get Activation Status
      operationId: configmedialivev1livedomainversionversionidactivation
      x-api-path-slug: configmedialivev1livedomainversionversionidactivation-get
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: versionId
        description: Domain&#8217;s incremental version number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Version
      - Activation
    put:
      summary: Activate a Version
      description: Activate a Version
      operationId: configmedialivev1livedomainversionversionidactivation
      x-api-path-slug: configmedialivev1livedomainversionversionidactivation-put
      parameters:
      - in: query
        name: domain
        description: Unique identifier for each domain
        type: string
      - in: query
        name: versionId
        description: Domain&#8217;s incremental version number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Domain
      - Version
      - Activation
  /config-media-live/v1/api/live/utils/archivelocation:
    get:
      summary: List Archive Locations
      description: List Archive Locations
      operationId: configmedialivev1apiliveutilsarchivelocation
      x-api-path-slug: configmedialivev1apiliveutilsarchivelocation-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Archives
  /config-media-live/v1/live/utils/contacts:
    get:
      summary: List Contacts
      description: List Contacts
      operationId: configmedialivev1liveutilscontacts
      x-api-path-slug: configmedialivev1liveutilscontacts-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Contacts
  /config-media-live/v1/live/utils/countries:
    get:
      summary: List Countries
      description: List Countries
      operationId: configmedialivev1liveutilscountries
      x-api-path-slug: configmedialivev1liveutilscountries-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Countries
  /config-media-live/v1/live/utils/cpcode:
    get:
      summary: List CP Codes
      description: List CP Codes
      operationId: configmedialivev1liveutilscpcode
      x-api-path-slug: configmedialivev1liveutilscpcode-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Cpcode
  /config-media-live/v1/live/utils/delivery/format:
    get:
      summary: List Delivery Formats
      description: List Delivery Formats
      operationId: configmedialivev1liveutilsdeliveryformat
      x-api-path-slug: configmedialivev1liveutilsdeliveryformat-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Delivery
      - Format
  /config-media-live/v1/live/utils/ingest/format:
    get:
      summary: List Ingest Formats
      description: List Ingest Formats
      operationId: configmedialivev1liveutilsingestformat
      x-api-path-slug: configmedialivev1liveutilsingestformat-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Live
      - Live
      - Utils
      - Ingest
      - Format
  /config-saas-registration/v1/applications/:
    get:
      summary: List Applications
      description: List Applications
      operationId: configsaasregistrationv1applicationscontractid
      x-api-path-slug: configsaasregistrationv1applications-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Applications
      - Contract
    post:
      summary: Create a New Application
      description: Create a New Application
      operationId: configsaasregistrationv1applicationscontractid
      x-api-path-slug: configsaasregistrationv1applications-post
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Applications
      - Contract
  /config-saas-registration/v1/applications/{surrogateId}/:
    get:
      summary: Get an Application
      description: Get an Application
      operationId: configsaasregistrationv1applicationssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1applicationssurrogateid-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Applications
      - Surrogate
      - Contract
    delete:
      summary: Remove an Application
      description: Remove an Application
      operationId: configsaasregistrationv1applicationssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1applicationssurrogateid-delete
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Applications
      - Surrogate
      - Contract
    put:
      summary: Modify an Application
      description: Modify an Application
      operationId: configsaasregistrationv1applicationssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1applicationssurrogateid-put
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Applications
      - Surrogate
      - Contract
  /config-saas-registration/v1/customers/:
    get:
      summary: List Customers
      description: List Customers
      operationId: configsaasregistrationv1customerscontractid
      x-api-path-slug: configsaasregistrationv1customers-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Customers
      - Contract
    post:
      summary: Create a New Customer
      description: Create a New Customer
      operationId: configsaasregistrationv1customerscontractid
      x-api-path-slug: configsaasregistrationv1customers-post
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Customers
      - Contract
  /config-saas-registration/v1/customers/{surrogateId}/:
    get:
      summary: Get a Customer
      description: Get a Customer
      operationId: configsaasregistrationv1customerssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1customerssurrogateid-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 456
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Customers
      - Surrogate
      - Contract
    delete:
      summary: Remove a Customer
      description: Remove a Customer
      operationId: configsaasregistrationv1customerssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1customerssurrogateid-delete
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 456
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Customers
      - Surrogate
      - Contract
    put:
      summary: Modify a Customer
      description: Modify a Customer
      operationId: configsaasregistrationv1customerssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1customerssurrogateid-put
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 456
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Customers
      - Surrogate
      - Contract
  /config-saas-registration/v1/pairs/:
    get:
      summary: List Pairs
      description: List Pairs
      operationId: configsaasregistrationv1pairscontractid
      x-api-path-slug: configsaasregistrationv1pairs-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Pairs
      - Contract
    post:
      summary: Create a New Pair
      description: Create a New Pair
      operationId: configsaasregistrationv1pairscontractid
      x-api-path-slug: configsaasregistrationv1pairs-post
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Pairs
      - Contract
  /config-saas-registration/v1/pairs/{surrogateId}/:
    get:
      summary: Get a Pair
      description: Get a Pair
      operationId: configsaasregistrationv1pairssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1pairssurrogateid-get
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Pairs
      - Surrogate
      - Contract
    delete:
      summary: Remove a Pair
      description: Remove a Pair
      operationId: configsaasregistrationv1pairssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1pairssurrogateid-delete
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Pairs
      - Surrogate
      - Contract
    put:
      summary: Modify a Pair
      description: Modify a Pair
      operationId: configsaasregistrationv1pairssurrogateidcontractid
      x-api-path-slug: configsaasregistrationv1pairssurrogateid-put
      parameters:
      - in: query
        name: contractId
        description: such as A-1234
        type: string
      - in: query
        name: surrogateId
        description: such as 123
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Saas
      - Registration
      - Pairs
      - Surrogate
      - Contract
  /config-media-security/v1/security:
    get:
      summary: List Policies
      description: List Policies
      operationId: configmediasecurityv1security
      x-api-path-slug: configmediasecurityv1security-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
    post:
      summary: Create a Policy
      description: Create a Policy
      operationId: configmediasecurityv1security
      x-api-path-slug: configmediasecurityv1security-post
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
  /config-media-security/v1/security/{policyID}:
    get:
      summary: Get a Policy
      description: Get a Policy
      operationId: configmediasecurityv1securitypolicyid
      x-api-path-slug: configmediasecurityv1securitypolicyid-get
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
    put:
      summary: Modify a Policy
      description: Modify a Policy
      operationId: configmediasecurityv1securitypolicyid
      x-api-path-slug: configmediasecurityv1securitypolicyid-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
    delete:
      summary: Mark a Policy for Deletion
      description: Mark a Policy for Deletion
      operationId: configmediasecurityv1securitypolicyid
      x-api-path-slug: configmediasecurityv1securitypolicyid-delete
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
  /config-media-security/v1/security/{policyID}/{environment}:
    get:
      summary: Get Policy per Environment
      description: Get Policy per Environment
      operationId: configmediasecurityv1securitypolicyidenvironment
      x-api-path-slug: configmediasecurityv1securitypolicyidenvironment-get
      parameters:
      - in: query
        name: environment
        description: The environment
        type: string
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Environment
  /config-media-security/v1/security/{policyID}/clonePolicy:
    post:
      summary: Clone a Policy
      description: Clone a Policy
      operationId: configmediasecurityv1securitypolicyidclonepolicy
      x-api-path-slug: configmediasecurityv1securitypolicyidclonepolicy-post
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Clonepolicy
  /config-media-security/v1/security/{policyID}/promote:
    put:
      summary: Promote a Policy
      description: Promote a Policy
      operationId: configmediasecurityv1securitypolicyidpromote
      x-api-path-slug: configmediasecurityv1securitypolicyidpromote-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Promote
  /config-media-security/v1/security/{policyID}/promoteDelete:
    delete:
      summary: Remove a Policy
      description: Remove a Policy
      operationId: configmediasecurityv1securitypolicyidpromotedelete
      x-api-path-slug: configmediasecurityv1securitypolicyidpromotedelete-delete
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Promotedelete
  /config-media-security/v1/security/{policyID}/revertDelete:
    put:
      summary: Restore a Policy Deletion
      description: Restore a Policy Deletion
      operationId: configmediasecurityv1securitypolicyidrevertdelete
      x-api-path-slug: configmediasecurityv1securitypolicyidrevertdelete-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Revertdelete
  /config-media-security/v1/security/{policyID}/revertEdit:
    put:
      summary: Restore a Policy Edit
      description: Restore a Policy Edit
      operationId: configmediasecurityv1securitypolicyidrevertedit
      x-api-path-slug: configmediasecurityv1securitypolicyidrevertedit-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Policy
      - Revertedit
  /config-media-security/v1/security/live/{domain}/policy:
    get:
      summary: Get an HD Config Policy
      description: Get an HD Config Policy
      operationId: configmediasecurityv1securitylivedomainpolicy
      x-api-path-slug: configmediasecurityv1securitylivedomainpolicy-get
      parameters:
      - in: query
        name: domain
        description: The fully qualified domain name for the host in question
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Domain
      - Policy
    put:
      summary: Modify an HD Config Policy
      description: Modify an HD Config Policy
      operationId: configmediasecurityv1securitylivedomainpolicy
      x-api-path-slug: configmediasecurityv1securitylivedomainpolicy-put
      parameters:
      - in: query
        name: domain
        description: The fully qualified domain name for the host in question
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Domain
      - Policy
  /config-media-security/v1/security/live/{domain}/policy/{environment}:
    get:
      summary: Get an HD Config Policy per Environment
      description: Get an HD Config Policy per Environment
      operationId: configmediasecurityv1securitylivedomainpolicyenvironment
      x-api-path-slug: configmediasecurityv1securitylivedomainpolicyenvironment-get
      parameters:
      - in: query
        name: domain
        description: The fully qualified domain name for the host in question
        type: string
      - in: query
        name: environment
        description: The environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Domain
      - Policy
      - Environment
  /config-media-security/v1/security/live/{policyID}/policyassignments:
    get:
      summary: List Policy Assignments
      description: List Policy Assignments
      operationId: configmediasecurityv1securitylivepolicyidpolicyassignments
      x-api-path-slug: configmediasecurityv1securitylivepolicyidpolicyassignments-get
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Policy
      - Policyassignments
  /config-media-security/v1/security/live/{policyID}/policyassignments/{environment}:
    get:
      summary: Get a Policy Assignment
      description: Get a Policy Assignment
      operationId: configmediasecurityv1securitylivepolicyidpolicyassignmentsenvironment
      x-api-path-slug: configmediasecurityv1securitylivepolicyidpolicyassignmentsenvironment-get
      parameters:
      - in: query
        name: environment
        description: The environment
        type: string
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Policy
      - Policyassignments
      - Environment
  /config-media-security/v1/security/live/{policyID}/policyassignments/promote:
    put:
      summary: Promote a Policy Assignment
      description: Promote a Policy Assignment
      operationId: configmediasecurityv1securitylivepolicyidpolicyassignmentspromote
      x-api-path-slug: configmediasecurityv1securitylivepolicyidpolicyassignmentspromote-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Policy
      - Policyassignments
      - Promote
  /config-media-security/v1/security/live/{policyID}/policyassignments/revert:
    put:
      summary: Revert a Policy Assignment Promotion
      description: Revert a Policy Assignment Promotion
      operationId: configmediasecurityv1securitylivepolicyidpolicyassignmentsrevert
      x-api-path-slug: configmediasecurityv1securitylivepolicyidpolicyassignmentsrevert-put
      parameters:
      - in: query
        name: policyID
        description: The ID of the policy to fetch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Live
      - Policy
      - Policyassignments
      - Revert
  /config-media-security/v1/security/countries:
    get:
      summary: List Countries
      description: List Countries
      operationId: configmediasecurityv1securitycountries
      x-api-path-slug: configmediasecurityv1securitycountries-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Countries
  /config-media-security/v1/security/dmas:
    get:
      summary: List Designated Market Areas
      description: List Designated Market Areas
      operationId: configmediasecurityv1securitydmas
      x-api-path-slug: configmediasecurityv1securitydmas-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Dmas
  /config-media-security/v1/security/regions:
    get:
      summary: List Regions
      description: List Regions
      operationId: configmediasecurityv1securityregions
      x-api-path-slug: configmediasecurityv1securityregions-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Regions
  /config-media-security/v1/security/regions/{countryCode}:
    get:
      summary: List Regions per Country
      description: List Regions per Country
      operationId: configmediasecurityv1securityregionscountrycode
      x-api-path-slug: configmediasecurityv1securityregionscountrycode-get
      parameters:
      - in: query
        name: countryCode
        description: The country code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Regions
      - Countrycode
  /config-media-security/v1/security/acgs:
    get:
      summary: List Access Control Groups
      description: List Access Control Groups
      operationId: configmediasecurityv1securityacgs
      x-api-path-slug: configmediasecurityv1securityacgs-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Media
      - Security
      - Security
      - Acgs
  /config-secure-provisioning-service/v1/sps-requests:
    post:
      summary: Create a Request
      description: Create a Request
      operationId: configsecureprovisioningservicev1spsrequestscontractidgroupidafterinformation
      x-api-path-slug: configsecureprovisioningservicev1spsrequests-post
      parameters:
      - in: query
        name: after
        description: If specified for GET requests, returns only the SPS requests
          created after the date entered
        type: string
      - in: query
        name: contractId
        description: For POST requests, the ID of the contract associated with the
          new policy
        type: string
      - in: query
        name: groupId
        description: For POST requests, the ID of the group associated with the new
          policy
        type: string
      - in: query
        name: information
        description: If specified for GET requests, returns parameters posted with
          the SPS request resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Secure
      - Provisioning
      - Service
      - Sps
      - Requests
      - Contract
      - group
      - after
      - information
    get:
      summary: List SPS Requests
      description: List SPS Requests
      operationId: configsecureprovisioningservicev1spsrequestscontractidgroupidafterinformation
      x-api-path-slug: configsecureprovisioningservicev1spsrequests-get
      parameters:
      - in: query
        name: after
        description: If specified for GET requests, returns only the SPS requests
          created after the date entered
        type: string
      - in: query
        name: contractId
        description: For POST requests, the ID of the contract associated with the
          new policy
        type: string
      - in: query
        name: groupId
        description: For POST requests, the ID of the group associated with the new
          policy
        type: string
      - in: query
        name: information
        description: If specified for GET requests, returns parameters posted with
          the SPS request resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Secure
      - Provisioning
      - Service
      - Sps
      - Requests
      - Contract
      - group
      - after
      - information
  /config-gtm/v1/domains/:
    get:
      summary: List Domains
      description: List Domains
      operationId: configgtmv1domains
      x-api-path-slug: configgtmv1domains-get
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Gtm
      - Domains
  /config-gtm/v1/domains/{domain}:
    get:
      summary: Get a Domain
      description: Get a Domain
      operationId: configgtmv1domainsdomain
      x-api-path-slug: configgtmv1domainsdomain-get
      parameters:
      - in: query
        name: domain
        description: Name of Traffic Management domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configurations
      - Gtm
      - Domains
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