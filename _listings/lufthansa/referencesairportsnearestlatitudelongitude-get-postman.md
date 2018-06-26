{
  "info": {
    "name": "LH Public Nearest Airports",
    "_postman_id": "c61645c3-dcd4-4487-addb-daa8665b6304",
    "description": "List the 5 closest airports to the given latitude and longitude, irrespective of the radius of the reference point.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "References",
      "item": [
        {
          "id": "35b5bf61-a4d9-4ab2-a657-c56f4cf1c27b",
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
              "id": "463aa9fe-4ecd-4f06-80f4-c9a87c664fb4"
            }
          ]
        }
      ]
    }
  ]
}