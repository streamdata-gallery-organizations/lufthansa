---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Cities
  version: "1.0"
  description: List all cities or one specific city. It is possible to request the
    response in a specific language.
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
  /operations/flightstatus/departures/{airportCode}/{fromDateTime}:
    get:
      summary: Flight Status at Departure Airport
      description: Status of all departures from a given airport up to 4 hours from
        the provided date time.
      operationId: OperationsFlightstatusDeparturesByAirportCodeAndFromDateTimeGet
      x-api-path-slug: operationsflightstatusdeparturesairportcodefromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: Departure airport
      - in: path
        name: fromDateTime
        description: Start of time range in local time of departure airport (YYYY-MM-DDTHH:mm)
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
      - Departures
      - AirportCode
      - FromDateTime
  /operations/flightstatus/route/{origin}/{destination}/{date}:
    get:
      summary: Flight Status by Route
      description: Status of flights between a given origin and destination on a given
        date.
      operationId: OperationsFlightstatusRouteDateByOriginAndDestinationGet
      x-api-path-slug: operationsflightstatusrouteorigindestinationdate-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: date
        description: Departure date (YYYY-MM-DD) in local time of departure airport
      - in: path
        name: destination
        description: 3-letter IATA airport code (e
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: 3-letter IATA airport (e
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Flightstatus
      - Route
      - Origin
      - Destination
      - Date
  /operations/flightstatus/{flightNumber}/{date}:
    get:
      summary: Flight Status
      description: Status of a particular flight (boarding, delayed, etc.).
      operationId: OperationsFlightstatusByFlightNumberAndDateGet
      x-api-path-slug: operationsflightstatusflightnumberdate-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: date
        description: The departure date (YYYY-MM-DD) in the local time of the departure
          airport
      - in: path
        name: flightNumber
        description: Flight number including carrier code and any suffix (e
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
      - FlightNumber
      - Date
  /operations/schedules/{origin}/{destination}/{fromDateTime}:
    get:
      summary: Flight Schedules
      description: Scheduled flights between given airports on a given date.
      operationId: OperationsSchedulesFromDateTimeByOriginAndDestinationGet
      x-api-path-slug: operationsschedulesorigindestinationfromdatetime-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: destination
        description: Destination airport
      - in: query
        name: directFlights
        description: Show only direct flights (false=0, true=1)
      - in: path
        name: fromDateTime
        description: Local departure date and optionally departure time (YYYY-MM-DD
          or YYYY-MM-DDTHH:mm)
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: Departure airport
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Schedules
      - Origin
      - Destination
      - FromDateTime
  /references/aircraft/{aircraftCode}:
    get:
      summary: Aircraft
      description: List all aircraft types or one specific aircraft type.
      operationId: ReferencesAircraftByAircraftCodeGet
      x-api-path-slug: referencesaircraftaircraftcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: aircraftCode
        description: 3-character IATA aircraft code
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
      - References
      - Aircraft
      - AircraftCode
  /references/airlines/{airlineCode}:
    get:
      summary: Airlines
      description: List all airlines or one specific airline.
      operationId: ReferencesAirlinesByAirlineCodeGet
      x-api-path-slug: referencesairlinesairlinecode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airlineCode
        description: 2-character IATA airline/carrier code
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
      - References
      - Airlines
      - AirlineCode
  /references/airports/nearest/{latitude},{longitude}:
    get:
      summary: Nearest Airports
      description: List the 5 closest airports to the given latitude and longitude,
        irrespective of the radius of the reference point.
      operationId: ReferencesAirportsNearestByLatitudeAndLongitudeGet
      x-api-path-slug: referencesairportsnearestlatitudelongitude-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
      - in: path
        name: latitude
        description: Latitude in decimal format to at most 3 decimal places
      - in: path
        name: longitude
        description: Longitude in decimal format to at most 3 decimal places
      responses:
        200:
          description: OK
      tags:
      - References
      - Airports
      - Nearest
      - Latitude
      - Longitude
  /references/airports/{airportCode}:
    get:
      summary: Airports
      description: List all airports or one specific airport. All airports response
        is very large. It is possible to request the response in a specific language.
      operationId: ReferencesAirportsByAirportCodeGet
      x-api-path-slug: referencesairportsairportcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: 3-letter IATA airport code
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: LHoperated
        description: Restrict the results to locations with flights operated by LH
          (false=0, true=1)
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
      - References
      - Airports
      - AirportCode
  /references/cities/{cityCode}:
    get:
      summary: Cities
      description: List all cities or one specific city. It is possible to request
        the response in a specific language.
      operationId: ReferencesCitiesByCityCodeGet
      x-api-path-slug: referencescitiescitycode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: cityCode
        description: 3-letter IATA city code
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
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
      - References
      - Cities
      - CityCode
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