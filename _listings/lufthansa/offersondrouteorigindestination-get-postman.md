{
  "info": {
    "name": "LH Partner OND Route",
    "_postman_id": "e8db0990-2399-45a7-ad27-147f4f40d862",
    "description": "Returns LH route origin & destination information",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baggage",
      "item": [
        {
          "id": "445a606e-6557-466b-8573-fcb9b1e4c549",
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
              "id": "a881c22f-5699-420a-ac0f-8397f6ad341b"
            }
          ]
        }
      ]
    },
    {
      "name": "All",
      "item": [
        {
          "id": "4766df6d-b146-4e21-8329-4c06a1a2ae00",
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
              "id": "8b2e00a5-866c-4424-b70f-5b160997cc2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Best",
      "item": [
        {
          "id": "5b2a68a9-b5dc-4993-888c-5e2582bb80d3",
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
              "id": "2693b341-e13a-4d4d-8c08-ef62bea9f698"
            }
          ]
        }
      ]
    },
    {
      "name": "Deep",
      "item": [
        {
          "id": "26c04932-e8d7-40ef-808f-5554ac29491e",
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
              "id": "bba93caa-be62-4775-80c7-bc3848f84f7b"
            }
          ]
        }
      ]
    },
    {
      "name": "LH",
      "item": [
        {
          "id": "2285994f-fd26-4d99-bae7-46320b0e9359",
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
              "id": "6142faac-5549-4667-a9e8-c3eaf12db520"
            }
          ]
        },
        {
          "id": "dad4ab6a-1b63-4e20-acc4-c47dec8a3ff1",
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
              "id": "053acccf-e52c-4f78-9cbc-5fe1c5f6b502"
            }
          ]
        }
      ]
    },
    {
      "name": "Fares",
      "item": [
        {
          "id": "e898be08-fc0a-4ad4-88ff-c26a0e157553",
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
              "id": "64cc2f79-8da2-403e-9c22-c3e5a2d7550c"
            }
          ]
        },
        {
          "id": "8e917186-c67a-4aec-9626-2e819bdfa593",
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
              "id": "dc5753eb-5e40-442d-95ba-4b04ee571d70"
            }
          ]
        }
      ]
    },
    {
      "name": "Lowest",
      "item": [
        {
          "id": "c56d900b-1986-4b14-ab7d-5ac2ce282429",
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
              "id": "ec7b96b4-ed20-471a-8d48-9fbeb4664f68"
            }
          ]
        }
      ]
    },
    {
      "name": "OND",
      "item": [
        {
          "id": "4ebb092c-5e05-409d-87b1-3e60ecc34b5a",
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
              "id": "a678d3eb-82a6-4444-a5a6-5ff59e237bfc"
            }
          ]
        }
      ]
    }
  ]
}