{
  "info": {
    "name": "LH Public Seat Maps",
    "_postman_id": "af232c5b-0c9f-446e-b8e6-b00f443a56f6",
    "description": "Cabin layout and seat characteristics.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Offers",
      "item": [
        {
          "id": "88465b36-4f89-4e7d-b228-de11af1094bf",
          "name": "OffersSeatmapsDestinationDateCabinClassByFlightNumberAndOriginGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "offers/seatmaps/:flightNumber/:origin/:destination/:date/:cabinClass"
              ],
              "variable": [
                {
                  "id": "cabinClass",
                  "value": "{}",
                  "type": "string"
                },
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
                  "id": "flightNumber",
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
            "description": "Cabin layout and seat characteristics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "057d8eff-9c92-40b9-8f43-4608d1ec1879"
            }
          ]
        }
      ]
    }
  ]
}