{
  "info": {
    "name": "LH Public Airlines",
    "_postman_id": "7a38d350-9a6e-47b2-a9bb-f8f4125aed41",
    "description": "List all airlines or one specific airline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "References",
      "item": [
        {
          "id": "f253c3a2-eea8-442d-9e1f-5311a74fcf89",
          "name": "ReferencesAirlinesByAirlineCodeGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "references/airlines/:airlineCode"
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
                  "id": "airlineCode",
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
            "description": "List all airlines or one specific airline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6eaf028-3b7f-4d22-95fd-c04a8b42287f"
            }
          ]
        }
      ]
    }
  ]
}