{
  "info": {
    "name": "LH Partner Price Offers",
    "_postman_id": "1eccf0fb-585d-4215-b5b3-67e000df9c64",
    "description": "Retrieve a best price offer given an origin and destination.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baggage",
      "item": [
        {
          "id": "49762394-78dd-4b97-bc1d-4fc68c3e714d",
          "name": "baggage.baggagetripandcontact.searchID.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "baggage/baggagetripandcontact/:searchID"
              ],
              "variable": [
                {
                  "id": "searchID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve passenger trip, contact and baggage details. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c85123b7-379e-4064-8021-5852891642c5"
            }
          ]
        }
      ]
    },
    {
      "name": "All",
      "item": [
        {
          "id": "9c89bfed-43ad-463d-9374-b67280c9ed23",
          "name": "offers.fares.allfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/allfares?cabin-class=%7B%7D&catalogues=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&return-date=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all available fares for a specific Origin & Destination pair on a given date. Available fares are: One-way and Return for 4U. Return only for OS"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a62428d-b6e0-4639-8318-b6e9dd435331"
            }
          ]
        }
      ]
    },
    {
      "name": "Best",
      "item": [
        {
          "id": "047aa384-2d8e-41d3-b4bf-678b979f2bbb",
          "name": "offers.fares.bestfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/bestfares?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&range=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&trip-duration=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve best fares for the requested journey across multiple days or multiple months."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7178ad52-30c3-484b-a1ef-22abdbe355aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Deep",
      "item": [
        {
          "id": "609b2f6d-55aa-4395-8e9d-5175c208abc3",
          "name": "offers.fares.deeplink.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&destination-name=%7B%7D&encryption-key=%7B%7D&fare=%7B%7D&fare-currency=%7B%7D&lang=%7B%7D&net-fare=%7B%7D&origin=%7B%7D&origin-name=%7B%7D&outbound-segments=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&return-segments=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid deep links for the provided input parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "530e5635-947b-4844-bf4e-effd73703f66"
            }
          ]
        }
      ]
    },
    {
      "name": "LH",
      "item": [
        {
          "id": "5dd7845a-7680-4a6a-b4a0-cd255cf3fa28",
          "name": "offers.fares.deeplink.ffp.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink/ffp?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&encryption-key=%7B%7D&lang=%7B%7D&origin=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid LH deep links (FFP - links to flight selection screen on LH.COM)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea5a4e88-2aa1-442a-9c15-f12030c6deae"
            }
          ]
        },
        {
          "id": "e3295faa-3e9f-4dd8-aea3-c3e7d4c771f1",
          "name": "offers.fares.deeplink.itco.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink/itco?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&encryption-key=%7B%7D&fare=%7B%7D&fare-currency=%7B%7D&lang=%7B%7D&net-fare=%7B%7D&origin=%7B%7D&outbound-segments=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&return-segments=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f21f9f2-dd6e-4f0f-b753-14daff76995f"
            }
          ]
        }
      ]
    },
    {
      "name": "Fares",
      "item": [
        {
          "id": "4b422e47-70f8-4671-98ad-992283771c0e",
          "name": "Fares",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/fares?carriers=%7B%7D&catalogues=%7B%7D&fare-types=%7B%7D&segments=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all available fares per fare family for a specific Origin & Destination on a given date"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59026387-eb06-4db2-9f65-4c6632a032a2"
            }
          ]
        },
        {
          "id": "620b5a42-edae-4073-8e25-d50362225510",
          "name": "offers.fares.subscriptions.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/subscriptions?cabin-class=%7B%7D&country=%7B%7D&destination=%7B%7D&email=%7B%7D&lang=%7B%7D&origin=%7B%7D&trackingid=%7B%7D&trip-duration=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create a subscription for best price O&D. Receive regular updates on lowest fares"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1652872-7d4a-4c4e-b6b8-16868f9ecffd"
            }
          ]
        }
      ]
    },
    {
      "name": "Lowest",
      "item": [
        {
          "id": "03760783-5f29-4ac9-994a-b9e43a9afda4",
          "name": "offers.fares.lowestfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/lowestfares?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&return-date=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve lowest fare for a specific Origin & Destination pair on a given date. Available fares are: One-way and Return for 4U. Return only for OS & LH"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0a027ad-0bd3-4fa8-a319-6be5fe3dced0"
            }
          ]
        }
      ]
    },
    {
      "name": "OND",
      "item": [
        {
          "id": "8662ce52-9cf6-4685-a831-680e2e36b53f",
          "name": "offers.ond.route.origin.destination.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "offers/ond/route/:origin/:destination"
              ],
              "query": [
                {
                  "key": "catalogues",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "destination",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "origin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH route origin & destination information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed34a0b7-c2ac-4d81-a4c2-c32aa35da6bf"
            }
          ]
        },
        {
          "id": "f14a23cc-a64c-4d5e-b6ad-22b9b2c19582",
          "name": "offers.ond.status.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/ond/status?catalogues=%7B%7D&new-routes=%7B%7D&old-routes=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH network route status information. Search for recently added or retired routes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d1f3d28-b227-4d4b-8a6f-934ff9a434cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "218a3606-4800-42b1-9e04-6e5a374572e7",
          "name": "offers.ond.top.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/ond/top?catalogues=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH Top routes per country or across all countries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50352078-6c4a-47e4-b739-b24b450c7097"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "8172b8c8-8e28-46ef-b915-c3e84f6ef2a0",
          "name": "Orders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "orders/orders/:orderID/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "orderID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve order by ID and optionally name. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e12c838-a3aa-4ed9-aa70-b24ccd8ed260"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto",
      "item": [
        {
          "id": "a022cb00-10fb-4d33-823a-4486e614360f",
          "name": "preflight.autocheckin.ticketnumber.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "preflight/autocheckin/:ticketnumber"
              ],
              "query": [
                {
                  "key": "emailAddress",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ticketnumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Trigger an automatic check-in given a ticket number. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17d3afa6-8863-42a5-8a9c-2bc8a23c3f99"
            }
          ]
        }
      ]
    },
    {
      "name": "Price",
      "item": [
        {
          "id": "8a67ae46-9a49-4a6d-8b29-a2f7cca55ceb",
          "name": "promotions.priceoffers.flights.ond.origin.destination.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "promotions/priceoffers/flights/ond/:origin/:destination"
              ],
              "query": [
                {
                  "key": "departureDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "returnDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "destination",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "origin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a best price offer given an origin and destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79c9c650-8e7d-4088-970e-bc5abf491e89"
            }
          ]
        }
      ]
    }
  ]
}