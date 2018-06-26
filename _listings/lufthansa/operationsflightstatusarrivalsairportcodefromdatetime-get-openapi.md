---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Flight Status at Arrival Airport
  version: "1.0"
  description: Status of all arrivals at a given airport up to 4 hours from the provided
    date time.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cargo/getRoute/{origin}-{destination}/{fromDate}/{productCode}:
    get:
      summary: Retrieve all flights
      description: Retrieve a list of all possible flights (both direct and connecting)
        between two airports on a given date. Routes are available for today and up
        to days in the future.
      operationId: CargoGetRouteFromDateProductCodeByOriginAndDestinationGet
      x-api-path-slug: cargogetrouteorigindestinationfromdateproductcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: destination
        description: 'Arrival airport : 3-letter IATA airport code, e'
      - in: path
        name: fromDate
        description: Departure date in the local time of the departure airport
      - in: path
        name: origin
        description: 'Departure Airport : 3-letter IATA airport code, e'
      - in: path
        name: productCode
        description: 'Product code for requested service and specials : 3-letter eg:
          YNZ'
      responses:
        200:
          description: OK
      tags:
      - Cargo
      - GetRoute
      - Origin
      - Destination
      - FromDate
      - ProductCode
  /cargo/shipmentTracking/{aWBPrefix}-{aWBNumber}:
    get:
      summary: Shipment Tracking
      description: With this tracking service you can easily retrieve your shipment
        or flight status information.
      operationId: CargoShipmentTrackingByAWBPrefixAndAWBNumberGet
      x-api-path-slug: cargoshipmenttrackingawbprefixawbnumber-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: aWBNumber
        description: 'aWBNumber : The Air Waybill Number , format : [0-9]{8} e'
      - in: path
        name: aWBPrefix
        description: 'aWBPrefix : Represents the airline that is the owner of this
          AWB, i'
      responses:
        200:
          description: OK
      tags:
      - Cargo
      - ShipmentTracking
      - AWBPrefix
      - AWBNumber
  /offers/lounges/{location}:
    get:
      summary: Lounges
      description: Lounge information
      operationId: OffersLoungesByLocationGet
      x-api-path-slug: offersloungeslocation-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabinClass
        description: 'Cabin class: M, E, C, F (Acceptable values are: , M, E, C, F)'
      - in: query
        name: lang
        description: Language code
      - in: path
        name: location
        description: 3-leter IATA airport or city code (e
      - in: query
        name: tierCode
        description: 'Frequent flyer level (FTL, SGC, SEN, HON) (Acceptable values
          are: , FTL, SGC, SEN, HON)'
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Lounges
      - Location
  /offers/seatmaps/{flightNumber}/{origin}/{destination}/{date}/{cabinClass}:
    get:
      summary: Seat Maps
      description: Cabin layout and seat characteristics.
      operationId: OffersSeatmapsDestinationDateCabinClassByFlightNumberAndOriginGet
      x-api-path-slug: offersseatmapsflightnumberorigindestinationdatecabinclass-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: cabinClass
        description: 'Cabin class: M, E, C, F'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD)
      - in: path
        name: destination
        description: Destination airport
      - in: path
        name: flightNumber
        description: Flight number including carrier code and any suffix (e
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Offers
      - Seatmaps
      - FlightNumber
      - Origin
      - Destination
      - Date
      - CabinClass
  /operations/flightstatus/arrivals/{airportCode}/{fromDateTime}:
    get:
      summary: Flight Status at Arrival Airport
      description: Status of all arrivals at a given airport up to 4 hours from the
        provided date time.
      operationId: OperationsFlightstatusArrivalsByAirportCodeAndFromDateTimeGet
      x-api-path-slug: operationsflightstatusarrivalsairportcodefromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: 3-letter IATA aiport code (e
      - in: path
        name: fromDateTime
        description: Start of time range in local time of arrival airport (YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Arrivals
      - AirportCode
      - FromDateTime
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