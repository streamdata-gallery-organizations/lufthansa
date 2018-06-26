{
  "info": {
    "name": "LH Public Flight Schedules",
    "_postman_id": "10f8033b-578a-402f-9feb-00d2e505dde0",
    "description": "Scheduled flights between given airports on a given date.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cargo",
      "item": [
        {
          "id": "577a5485-864b-4538-a6e4-64f5222eb26e",
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
              "id": "2f9d6085-5cd6-4dc3-bf4b-ea29b0021a7a"
            }
          ]
        }
      ]
    },
    {
      "name": "Operations",
      "item": [
        {
          "id": "3cdec972-94b9-4079-a2c3-255b1e0b67a3",
          "name": "OperationsFlightstatusArrivalsByAirportCodeAndFromDateTimeGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "operations/flightstatus/arrivals/:airportCode/:fromDateTime"
              ],
              "query": [
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
                  "id": "airportCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "fromDateTime",
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
            "description": "Status of all arrivals at a given airport up to 4 hours from the provided date time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9655d85d-9524-4c30-a0e5-59dfbf72f6cb"
            }
          ]
        },
        {
          "id": "a5fbe024-d99a-4272-aad0-00acc8642239",
          "name": "OperationsFlightstatusDeparturesByAirportCodeAndFromDateTimeGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "operations/flightstatus/departures/:airportCode/:fromDateTime"
              ],
              "query": [
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
                  "id": "airportCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "fromDateTime",
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
            "description": "Status of all departures from a given airport up to 4 hours from the provided date time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ce7d756-7078-4aa9-87dc-7460a40fa8ec"
            }
          ]
        },
        {
          "id": "4da54e26-08e4-48b3-bc1d-b19d9c3cc4fc",
          "name": "OperationsSchedulesFromDateTimeByOriginAndDestinationGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "operations/schedules/:origin/:destination/:fromDateTime"
              ],
              "query": [
                {
                  "key": "directFlights",
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
                  "id": "fromDateTime",
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
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Scheduled flights between given airports on a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "663036a5-949e-44db-a9f6-4baf4a44a8a6"
            }
          ]
        }
      ]
    }
  ]
}