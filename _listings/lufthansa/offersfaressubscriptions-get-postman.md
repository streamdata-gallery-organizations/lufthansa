{
  "info": {
    "name": "LH Partner Fares Subscriptions",
    "_postman_id": "4a263e04-a2f4-45df-b68f-b7314426083a",
    "description": "Create a subscription for best price O&D. Receive regular updates on lowest fares",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fares",
      "item": [
        {
          "id": "665bbc06-9e76-4cad-984a-458cdcb87fa6",
          "name": "offers.fares.subscriptions.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/subscriptions?cabin-class=%7B%7D&country=%7B%7D&destination=%7B%7D&email=%7B%7D&lang=%7B%7D&origin=%7B%7D&trackingid=%7B%7D&trip-duration=%7B%7D",
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
            "description": "Create a subscription for best price O&D. Receive regular updates on lowest fares"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "523c8ec9-8fbf-4deb-9521-b745901fd83e"
            }
          ]
        }
      ]
    }
  ]
}