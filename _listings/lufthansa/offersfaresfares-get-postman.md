{
  "info": {
    "name": "LH Partner Fares",
    "_postman_id": "d13c832e-607a-4323-8911-af331cf4b168",
    "description": "Retrieve all available fares per fare family for a specific Origin & Destination on a given date",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baggage",
      "item": [
        {
          "id": "aca0fb58-8d3e-4c7f-80c7-d76ba1e3e70d",
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
              "id": "8e70bc12-5bea-4ae4-b5b9-62b2896bfd3e"
            }
          ]
        }
      ]
    },
    {
      "name": "All",
      "item": [
        {
          "id": "50621f02-9bae-441b-8c74-8cbbdc7edeec",
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
              "id": "f9edd5c3-6569-41b1-8ae2-b0f616ac73d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Best",
      "item": [
        {
          "id": "e1b74b53-18fe-4a46-98d1-8023bea4a30d",
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
              "id": "5ab7396f-86c4-4ac3-b920-6361d6d71a5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Deep",
      "item": [
        {
          "id": "41873d65-d8d1-46e2-8faf-6aa2323aa64c",
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
              "id": "e12e63de-bee8-433e-81ba-c1fc1142baa2"
            }
          ]
        }
      ]
    },
    {
      "name": "LH",
      "item": [
        {
          "id": "959e517a-4917-4931-85a8-9765f8c349cb",
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
              "id": "51305517-a41b-4beb-91a0-4f4f953de032"
            }
          ]
        },
        {
          "id": "04174c4e-d95f-4e7d-b03d-66181819a567",
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
              "id": "45676cc0-f843-4ded-a711-ca9054950e4a"
            }
          ]
        }
      ]
    },
    {
      "name": "Fares",
      "item": [
        {
          "id": "e5bcee98-843f-479b-9bc7-b5f59a125a59",
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
              "id": "b22d178b-d56b-48af-9932-709b5d94a6b3"
            }
          ]
        }
      ]
    }
  ]
}