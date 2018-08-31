---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Retrieve all flights
  version: "1.0"
  description: Retrieve a list of all possible flights (both direct and connecting)
    between two airports on a given date. Routes are available for today and up to
    days in the future.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /baggage/baggagetripandcontact/{searchID}:
    get:
      summary: Baggage Trip and Contact
      description: Retrieve passenger trip, contact and baggage details. This service
        is only accessible for LH privileged partners
      operationId: baggage.baggagetripandcontact.searchID.get
      x-api-path-slug: baggagebaggagetripandcontactsearchid-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: searchID
        description: Bag tag number, PNR, boarding card or FQTV ID
      responses:
        200:
          description: OK
      tags:
      - Baggage
      - Trip
      - Contact
  /offers/fares/allfares:
    get:
      summary: All Fares
      description: 'Retrieves all available fares for a specific Origin & Destination
        pair on a given date. Available fares are: One-way and Return for 4U. Return
        only for OS'
      operationId: offers.fares.allfares.get
      x-api-path-slug: offersfaresallfares-get
      parameters:
      - in: header
        name: Accept
        description: 'Mandatory http header:  application/xml or application/json'
      - in: query
        name: cabin-class
        description: Enter the required cabin class (e
      - in: query
        name: catalogues
        description: Specifies in which catalogue the fares need to be searched (e
      - in: query
        name: destination
        description: Enter journey destination (e
      - in: query
        name: fare-family
        description: Mandatory for 4U
      - in: query
        name: origin
        description: Enter journey origin (e
      - in: query
        name: return-date
        description: Enter journey return-date (e
      - in: query
        name: trackingid
        description: Austrian Airlines only - specify the web tracking id to be used
          in OS Deep link
      - in: query
        name: travel-date
        description: Enter journey travel-date (e
      - in: query
        name: travelers
        description: Specifies the type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - All
      - Fares
  /offers/fares/bestfares:
    get:
      summary: Best Fares
      description: Retrieve best fares for the requested journey across multiple days
        or multiple months.
      operationId: offers.fares.bestfares.get
      x-api-path-slug: offersfaresbestfares-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Search fares from these carriers catalogues (e
      - in: query
        name: country
        description: Country code of requestor
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: fare-family
        description: 'Fare family: basic, smart, best, smartflex, bestflex - Germanwings
          only (Acceptable values are: , basic, smart, best, smartflex, bestflex)'
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: range
        description: 'Fare range: byday or bymonth (Acceptable values are: byday,
          bymonth)'
      - in: query
        name: trackingid
        description: Austrian Airlines only - specify the web tracking id to be used
          in OS Deep link
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: trip-duration
        description: Trip duration in days (e
      responses:
        200:
          description: OK
      tags:
      - Best
      - Fares
  /offers/fares/deeplink:
    get:
      summary: Deep Links
      description: Returns valid deep links for the provided input parameters
      operationId: offers.fares.deeplink.get
      x-api-path-slug: offersfaresdeeplink-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: destination-name
        description: Journey destination airport or city name (e
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: fare
        description: Travel fare (e
      - in: query
        name: fare-currency
        description: Fare currency (e
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: net-fare
        description: Travel net fare
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: origin-name
        description: Journey origin airport or city name (e
      - in: query
        name: outbound-segments
        description: Outbound flight segments in the sequence of travel (e
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: return-segments
        description: Flight segments in the sequence of travel (e
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - Deep
      - Links
  /offers/fares/deeplink/ffp:
    get:
      summary: LH Deep Links - FFP
      description: Returns valid LH deep links (FFP - links to flight selection screen
        on LH.COM)
      operationId: offers.fares.deeplink.ffp.get
      x-api-path-slug: offersfaresdeeplinkffp-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - LH
      - Deep
      - Links
      - '-'
      - FFP
  /offers/fares/deeplink/itco:
    get:
      summary: LH Deep Links - ITCO
      description: Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)
      operationId: offers.fares.deeplink.itco.get
      x-api-path-slug: offersfaresdeeplinkitco-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Carrier for which the deep link will be created (e
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: encryption-key
        description: Deep link encryption-key
      - in: query
        name: fare
        description: Travel fare (e
      - in: query
        name: fare-currency
        description: Fare currency (e
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: net-fare
        description: Travel net fare
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: outbound-segments
        description: Outbound flight segments in the sequence of travel (e
      - in: query
        name: partnerid
        description: Deep link partner id (e
      - in: query
        name: return-date
        description: Journey return-date (YYYY-MM-DD)
      - in: query
        name: return-segments
        description: Flight segments in the sequence of travel (e
      - in: query
        name: trackingid
        description: Deep link tracking ID
      - in: query
        name: travel-date
        description: Journey travel-date (YYYY-MM-DD)
      - in: query
        name: travelers
        description: Type and number of travelers (e
      responses:
        200:
          description: OK
      tags:
      - LH
      - Deep
      - Links
      - '-'
      - ITCO
  /offers/fares/fares:
    get:
      summary: Fares
      description: Retrieve all available fares per fare family for a specific Origin
        & Destination on a given date
      operationId: Fares
      x-api-path-slug: offersfaresfares-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: carriers
        description: Include fares for these carriers e
      - in: query
        name: catalogues
        description: Search fares from these carriers catalogues - currently active
          for Germanwings only  (4U)
      - in: query
        name: fare-types
        description: 'Fares family: basic,smart, best, smartflex, bestflex - Germanwings
          only (Acceptable values are: , basic, smart, best, smartflex, bestflex)'
      - in: query
        name: segments
        description: Journey details  e
      - in: query
        name: travelers
        description: Type and number of travelers e
      responses:
        200:
          description: OK
      tags:
      - Fares
  /offers/fares/lowestfares:
    get:
      summary: Lowest Fares
      description: 'Retrieve lowest fare for a specific Origin & Destination pair
        on a given date. Available fares are: One-way and Return for 4U. Return only
        for OS & LH'
      operationId: offers.fares.lowestfares.get
      x-api-path-slug: offersfareslowestfares-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: catalogues
        description: Search fares from these carriers catalogues e
      - in: query
        name: country
        description: Country code of requestor
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: fare-family
        description: 'Fare family: basic, smart, best, smartflex, bestflex - Germanwings
          only (Acceptable values are: , basic, smart, best, smartflex, bestflex)'
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: return-date
        description: Journey return-date - mandatory for OS and LH searches YYYY-MM-DD
      - in: query
        name: travel-date
        description: Journey travel-date YYYY-MM-DD
      - in: query
        name: travelers
        description: Type and number of travelers e
      responses:
        200:
          description: OK
      tags:
      - Lowest
      - Fares
  /offers/fares/subscriptions:
    get:
      summary: Fares Subscriptions
      description: Create a subscription for best price O&D. Receive regular updates
        on lowest fares
      operationId: offers.fares.subscriptions.get
      x-api-path-slug: offersfaressubscriptions-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: email
        description: Email Address)
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: trackingid
        description: Tracking parameter
      - in: query
        name: trip-duration
        description: Trip duration in days (e
      responses:
        200:
          description: OK
      tags:
      - Fares
      - Subscriptions
  /offers/ond/route/{origin}/{destination}:
    get:
      summary: OND Route
      description: Returns LH route origin & destination information
      operationId: offers.ond.route.origin.destination.get
      x-api-path-slug: offersondrouteorigindestination-get
      parameters:
      - in: header
        name: Accept
        description: 'Mandatory http header:  application/xml or application/json'
      - in: query
        name: catalogues
        description: Carrier for which the OND will be retrieved (e
      - in: path
        name: destination
        description: Enter either the destination city or country code (e
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      - in: path
        name: origin
        description: Enter either the orgin city or orgin country code (e
      responses:
        200:
          description: OK
      tags:
      - OND
      - Route
  /offers/ond/status:
    get:
      summary: OND Status
      description: Returns LH network route status information. Search for recently
        added or retired routes
      operationId: offers.ond.status.get
      x-api-path-slug: offersondstatus-get
      parameters:
      - in: header
        name: Accept
        description: 'Mandatory http header:  application/xml or application/json'
      - in: query
        name: catalogues
        description: Carrier for which the OND will be retrieved (e
      - in: query
        name: new-routes
        description: Enter if newly added routes should be returned in the response
      - in: query
        name: old-routes
        description: Enter if old (deleted) routes should be returned in the response
      responses:
        200:
          description: OK
      tags:
      - OND
      - Status
  /offers/ond/top:
    get:
      summary: Top OND
      description: Returns LH Top routes per country or across all countries
      operationId: offers.ond.top.get
      x-api-path-slug: offersondtop-get
      parameters:
      - in: header
        name: Accept
        description: 'Mandatory http header:  application/xml or application/json'
      - in: query
        name: catalogues
        description: Carrier for which the OND will be retrieved (e
      - in: query
        name: origin
        description: Enter the origin country code (e
      responses:
        200:
          description: OK
      tags:
      - Top
      - OND
  /orders/orders/{orderID}/{name}:
    get:
      summary: Orders
      description: Retrieve order by ID and optionally name. This service is only
        accessible for LH privileged partners
      operationId: Orders
      x-api-path-slug: ordersordersorderidname-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: name
        description: Surname of traveller
      - in: path
        name: orderID
        description: Unique order identifier
      responses:
        200:
          description: OK
      tags:
      - Orders
  /preflight/autocheckin/{ticketnumber}:
    put:
      summary: Auto Check-In
      description: Trigger an automatic check-in given a ticket number. This service
        is only accessible for LH privileged partners
      operationId: preflight.autocheckin.ticketnumber.put
      x-api-path-slug: preflightautocheckinticketnumber-put
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: emailAddress
        description: Email address
      - in: path
        name: ticketnumber
        description: Ticket number
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Check-In
  /promotions/priceoffers/flights/ond/{origin}/{destination}:
    get:
      summary: Price Offers
      description: Retrieve a best price offer given an origin and destination.
      operationId: promotions.priceoffers.flights.ond.origin.destination.get
      x-api-path-slug: promotionspriceoffersflightsondorigindestination-get
      parameters:
      - in: query
        name: departureDate
        description: Departure date in local time (YYYY-MM-DD)
      - in: path
        name: destination
        description: Destination city
      - in: path
        name: origin
        description: Departure city
      - in: query
        name: returnDate
        description: Return date in local time (YYYY-MM-DD)
      - in: query
        name: service
        description: Optional parameter
      responses:
        200:
          description: OK
      tags:
      - Price
      - Offers
  /references/seatdetails/{aircraftCode}/{cabinCode}:
    get:
      summary: Seat Details
      description: A description of all available seat details by aircraft type. You
        can retrieve the full set or details for a particular aircraft type.
      operationId: references.seatdetails.aircraftCode.cabinCode.get
      x-api-path-slug: referencesseatdetailsaircraftcodecabincode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: aircraftCode
        description: Aircraft type
      - in: path
        name: cabinCode
        description: 'Cabin class: M, E, C, F (Acceptable values are: , M, E, C, F)'
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      responses:
        200:
          description: OK
      tags:
      - Seat
      - Details
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