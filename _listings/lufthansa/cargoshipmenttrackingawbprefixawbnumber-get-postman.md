{
  "info": {
    "name": "LH Public Shipment Tracking",
    "_postman_id": "35d8bf30-2677-46f5-a2ff-c0d955da7c33",
    "description": "With this tracking service you can easily retrieve your shipment or flight status information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cargo",
      "item": [
        {
          "id": "4543e668-863f-4995-a13f-6dbf87870f32",
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
              "id": "ba87aade-5f82-44e5-9655-e4535fd3859b"
            }
          ]
        }
      ]
    }
  ]
}