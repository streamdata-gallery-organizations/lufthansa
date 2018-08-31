{
  "info": {
    "name": "LH Public Flight Status by Route",
    "_postman_id": "587c87f6-b7dd-4986-9469-1a422fab6116",
    "description": "Status of flights between a given origin and destination on a given date.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Operations",
      "item": [
        {
          "id": "e6bf04f9-43ad-4dca-9d16-03d1a67b4815",
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
              "id": "3285dbdc-56a7-4ebd-9ed2-1d476d8c2ec5"
            }
          ]
        },
        {
          "id": "4ecc75aa-cc82-4e1c-a99c-16901f123c39",
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
              "id": "b2861bb4-a3c2-45f2-90a2-94b525cbc36a"
            }
          ]
        },
        {
          "id": "fb4117dc-e734-4755-a9f2-63c390d65fd4",
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
              "id": "533109bc-b3d5-49a1-ad0d-902ece418383"
            }
          ]
        }
      ]
    }
  ]
}