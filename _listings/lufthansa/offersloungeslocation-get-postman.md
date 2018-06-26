{
  "info": {
    "name": "LH Public Lounges",
    "_postman_id": "2ce22c42-daa0-4b83-8229-c4e0c6578f9c",
    "description": "Lounge information",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cargo",
      "item": [
        {
          "id": "fbe7386d-a2b9-4223-b1a2-97c34a4c404c",
          "name": "CargoGetRouteFromDateProductCodeByOriginAndDestinationGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "cargo/getRoute/:origin-:destination/:fromDate/:productCode"
              ],
              "variable": [
                {
                  "id": "destination",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "fromDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "origin",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "productCode",
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
            "description": "Retrieve a list of all possible flights (both direct and connecting) between two airports on a given date. Routes are available for today and up to days in the future."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "817f9b08-5432-48a4-902f-bc647ad3f96b"
            }
          ]
        },
        {
          "id": "69fc50c2-ca42-4763-b94d-54a7141cde49",
          "name": "CargoShipmentTrackingByAWBPrefixAndAWBNumberGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "cargo/shipmentTracking/:aWBPrefix-:aWBNumber"
              ],
              "variable": [
                {
                  "id": "aWBNumber",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "aWBPrefix",
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
            "description": "With this tracking service you can easily retrieve your shipment or flight status information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd0c8bdf-5773-4578-b199-71c3b95119e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Offers",
      "item": [
        {
          "id": "e476fc31-9cf8-4568-981f-c1f62835748a",
          "name": "OffersLoungesByLocationGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "offers/lounges/:location"
              ],
              "query": [
                {
                  "key": "cabinClass",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tierCode",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "location",
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
            "description": "Lounge information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39cac9ca-81ac-49cc-8768-eda6f7af7e8e"
            }
          ]
        }
      ]
    }
  ]
}