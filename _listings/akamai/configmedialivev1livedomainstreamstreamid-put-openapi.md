---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API Modify a Stream
  description: Modify a Stream
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