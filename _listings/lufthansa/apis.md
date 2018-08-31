---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: Lufthansa
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Partner - Baggage Trip and Contact
  x-api-slug: baggagebaggagetripandcontactsearchid-get
  description: Retrieve passenger trip, contact and baggage details. This service
    is only accessible for LH privileged partners
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/baggagebaggagetripandcontactsearchid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/baggagebaggagetripandcontactsearchid-get-openapi.md
- name: LH Partner - All Fares
  x-api-slug: offersfaresallfares-get
  description: 'Retrieves all available fares for a specific Origin & Destination
    pair on a given date. Available fares are: One-way and Return for 4U. Return only
    for OS'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresallfares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresallfares-get-openapi.md
- name: LH Partner - Best Fares
  x-api-slug: offersfaresbestfares-get
  description: Retrieve best fares for the requested journey across multiple days
    or multiple months.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresbestfares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresbestfares-get-openapi.md
- name: LH Partner - Deep Links
  x-api-slug: offersfaresdeeplink-get
  description: Returns valid deep links for the provided input parameters
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplink-get-openapi.md
- name: LH Partner - LH Deep Links - FFP
  x-api-slug: offersfaresdeeplinkffp-get
  description: Returns valid LH deep links (FFP - links to flight selection screen
    on LH.COM)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplinkffp-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplinkffp-get-openapi.md
- name: LH Partner - LH Deep Links - ITCO
  x-api-slug: offersfaresdeeplinkitco-get
  description: Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplinkitco-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresdeeplinkitco-get-openapi.md
- name: LH Partner - Fares
  x-api-slug: offersfaresfares-get
  description: Retrieve all available fares per fare family for a specific Origin
    & Destination on a given date
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresfares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaresfares-get-openapi.md
- name: LH Partner - Lowest Fares
  x-api-slug: offersfareslowestfares-get
  description: 'Retrieve lowest fare for a specific Origin & Destination pair on a
    given date. Available fares are: One-way and Return for 4U. Return only for OS
    & LH'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfareslowestfares-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfareslowestfares-get-openapi.md
- name: LH Partner - Fares Subscriptions
  x-api-slug: offersfaressubscriptions-get
  description: Create a subscription for best price O&D. Receive regular updates on
    lowest fares
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaressubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersfaressubscriptions-get-openapi.md
- name: LH Partner - OND Route
  x-api-slug: offersondrouteorigindestination-get
  description: Returns LH route origin & destination information
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondrouteorigindestination-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondrouteorigindestination-get-openapi.md
- name: LH Partner - OND Status
  x-api-slug: offersondstatus-get
  description: Returns LH network route status information. Search for recently added
    or retired routes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondstatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondstatus-get-openapi.md
- name: LH Partner - Top OND
  x-api-slug: offersondtop-get
  description: Returns LH Top routes per country or across all countries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondtop-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersondtop-get-openapi.md
- name: LH Partner - Orders
  x-api-slug: ordersordersorderidname-get
  description: Retrieve order by ID and optionally name. This service is only accessible
    for LH privileged partners
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/ordersordersorderidname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/ordersordersorderidname-get-openapi.md
- name: LH Partner - Auto Check-In
  x-api-slug: preflightautocheckinticketnumber-put
  description: Trigger an automatic check-in given a ticket number. This service is
    only accessible for LH privileged partners
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/preflightautocheckinticketnumber-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/preflightautocheckinticketnumber-put-openapi.md
- name: LH Partner - Price Offers
  x-api-slug: promotionspriceoffersflightsondorigindestination-get
  description: Retrieve a best price offer given an origin and destination.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/promotionspriceoffersflightsondorigindestination-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/promotionspriceoffersflightsondorigindestination-get-openapi.md
- name: LH Partner - Seat Details
  x-api-slug: referencesseatdetailsaircraftcodecabincode-get
  description: A description of all available seat details by aircraft type. You can
    retrieve the full set or details for a particular aircraft type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesseatdetailsaircraftcodecabincode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesseatdetailsaircraftcodecabincode-get-openapi.md
- name: LH Public - Retrieve all flights
  x-api-slug: cargogetrouteorigindestinationfromdateproductcode-get
  description: Retrieve a list of all possible flights (both direct and connecting)
    between two airports on a given date. Routes are available for today and up to
    days in the future.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/cargogetrouteorigindestinationfromdateproductcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/cargogetrouteorigindestinationfromdateproductcode-get-openapi.md
- name: LH Public - Shipment Tracking
  x-api-slug: cargoshipmenttrackingawbprefixawbnumber-get
  description: With this tracking service you can easily retrieve your shipment or
    flight status information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/cargoshipmenttrackingawbprefixawbnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/cargoshipmenttrackingawbprefixawbnumber-get-openapi.md
- name: LH Public - Lounges
  x-api-slug: offersloungeslocation-get
  description: Lounge information
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersloungeslocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersloungeslocation-get-openapi.md
- name: LH Public - Seat Maps
  x-api-slug: offersseatmapsflightnumberorigindestinationdatecabinclass-get
  description: Cabin layout and seat characteristics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersseatmapsflightnumberorigindestinationdatecabinclass-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/offersseatmapsflightnumberorigindestinationdatecabinclass-get-openapi.md
- name: LH Public - Flight Status at Arrival Airport
  x-api-slug: operationsflightstatusarrivalsairportcodefromdatetime-get
  description: Status of all arrivals at a given airport up to 4 hours from the provided
    date time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusarrivalsairportcodefromdatetime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusarrivalsairportcodefromdatetime-get-openapi.md
- name: LH Public - Flight Status at Departure Airport
  x-api-slug: operationsflightstatusdeparturesairportcodefromdatetime-get
  description: Status of all departures from a given airport up to 4 hours from the
    provided date time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusdeparturesairportcodefromdatetime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusdeparturesairportcodefromdatetime-get-openapi.md
- name: LH Public - Flight Status by Route
  x-api-slug: operationsflightstatusrouteorigindestinationdate-get
  description: Status of flights between a given origin and destination on a given
    date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusrouteorigindestinationdate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusrouteorigindestinationdate-get-openapi.md
- name: LH Public - Flight Status
  x-api-slug: operationsflightstatusflightnumberdate-get
  description: Status of a particular flight (boarding, delayed, etc.).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusflightnumberdate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsflightstatusflightnumberdate-get-openapi.md
- name: LH Public - Flight Schedules
  x-api-slug: operationsschedulesorigindestinationfromdatetime-get
  description: Scheduled flights between given airports on a given date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsschedulesorigindestinationfromdatetime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/operationsschedulesorigindestinationfromdatetime-get-openapi.md
- name: LH Public - Aircraft
  x-api-slug: referencesaircraftaircraftcode-get
  description: List all aircraft types or one specific aircraft type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesaircraftaircraftcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesaircraftaircraftcode-get-openapi.md
- name: LH Public - Airlines
  x-api-slug: referencesairlinesairlinecode-get
  description: List all airlines or one specific airline.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairlinesairlinecode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairlinesairlinecode-get-openapi.md
- name: LH Public - Nearest Airports
  x-api-slug: referencesairportsnearestlatitudelongitude-get
  description: List the 5 closest airports to the given latitude and longitude, irrespective
    of the radius of the reference point.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-openapi.md
- name: LH Public - Airports
  x-api-slug: referencesairportsairportcode-get
  description: List all airports or one specific airport. All airports response is
    very large. It is possible to request the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairportsairportcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencesairportsairportcode-get-openapi.md
- name: LH Public - Cities
  x-api-slug: referencescitiescitycode-get
  description: List all cities or one specific city. It is possible to request the
    response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencescitiescitycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencescitiescitycode-get-openapi.md
- name: LH Public - Countries
  x-api-slug: referencescountriescountrycode-get
  description: List all countries or one specific country. It is possible to request
    the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencescountriescountrycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/lufthansa/master/_listings/lufthansa/referencescountriescountrycode-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://lota.data.api.gallery.streamdata.io
- type: x-api-stack
  url: http://lufthansa.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/lufthansa
- type: x-twitter
  url: https://twitter.com/lufthansa
- type: x-website
  url: http://lufthansa.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---