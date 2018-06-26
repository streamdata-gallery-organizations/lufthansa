{
  "info": {
    "name": "LH Public Airports",
    "_postman_id": "3bb49bd4-104f-4c1f-b298-91572a17d988",
    "description": "List all airports or one specific airport. All airports response is very large. It is possible to request the response in a specific language.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "References",
      "item": [
        {
          "id": "1445b5a2-5978-48d3-9bf2-4f7fb2137f24",
          "name": "ReferencesAirportsNearestByLatitudeAndLongitudeGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "references/airports/nearest/:latitude,:longitude"
              ],
              "query": [
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "latitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "longitude",
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
            "description": "List the 5 closest airports to the given latitude and longitude, irrespective of the radius of the reference point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16f210e1-3812-4c1a-8e07-c659ccc7d27b"
            }
          ]
        },
        {
          "id": "4f5dc8ef-61f7-4b85-a60d-861cc4543132",
          "name": "ReferencesAirportsByAirportCodeGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "references/airports/:airportCode"
              ],
              "query": [
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "LHoperated",
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
                  "id": "airportCode",
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
            "description": "List all airports or one specific airport. All airports response is very large. It is possible to request the response in a specific language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "667d188b-4005-4edd-aaa8-96eacd4b1191"
            }
          ]
        }
      ]
    }
  ]
}