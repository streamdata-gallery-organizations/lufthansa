---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Partner Deep Links
  version: "1.0"
  description: Returns valid deep links for the provided input parameters
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