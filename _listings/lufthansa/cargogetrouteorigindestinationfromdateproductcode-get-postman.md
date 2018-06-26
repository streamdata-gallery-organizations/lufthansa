{
  "info": {
    "name": "LH Public Retrieve all flights",
    "_postman_id": "6b88c184-b86c-4401-b2bf-80018aa7d063",
    "description": "Retrieve a list of all possible flights (both direct and connecting) between two airports on a given date. Routes are available for today and up to days in the future.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cargo",
      "item": [
        {
          "id": "686e20e3-f38a-4643-a73e-b4e56b2eb53f",
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
              "id": "e6fa6438-d959-4c17-8ee2-108fcbb90b67"
            }
          ]
        }
      ]
    }
  ]
}