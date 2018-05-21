---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API List Customers
  description: List Customers
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