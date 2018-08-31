{
  "info": {
    "name": "LH Public Flight Status",
    "_postman_id": "b2472532-0fb1-430f-9fcf-9b253d5def2c",
    "description": "Status of a particular flight (boarding, delayed, etc.).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Operations",
      "item": [
        {
          "id": "ee58ec29-4c7a-40f5-adf2-b060adc652e6",
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
              "id": "b22bfe3c-d109-4dca-b7e2-2c6dcd12baaf"
            }
          ]
        },
        {
          "id": "e285b02a-0fc0-4fb2-b41f-537c7c808c22",
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
              "id": "626ca6e6-0bae-4de2-bc63-332862e3185b"
            }
          ]
        },
        {
          "id": "f4b21c72-108a-4be4-9381-802a2bcab514",
          "name": "OperationsFlightstatusRouteDateByOriginAndDestinationGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "operations/flightstatus/route/:origin/:destination/:date"
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
                  "id": "date",
                  "value": "{}",
                  "type": "string"
                },
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
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Status of flights between a given origin and destination on a given date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "960f59fc-5084-4393-9c09-e89bc60e4ede"
            }
          ]
        },
        {
          "id": "0aa5535f-2946-4f4b-94a3-fba121fb4195",
          "name": "OperationsFlightstatusByFlightNumberAndDateGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "operations/flightstatus/:flightNumber/:date"
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
                  "id": "date",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "flightNumber",
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
            "description": "Status of a particular flight (boarding, delayed, etc.)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ed6de9f-1c4f-4841-acbb-49e902ae1a26"
            }
          ]
        }
      ]
    }
  ]
}