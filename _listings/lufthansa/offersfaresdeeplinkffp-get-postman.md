{
  "info": {
    "name": "LH Partner LH Deep Links - FFP",
    "_postman_id": "e0f0a075-3e4a-4597-b05e-61b1d2a5b36e",
    "description": "Returns valid LH deep links (FFP - links to flight selection screen on LH.COM)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deep",
      "item": [
        {
          "id": "70d67882-c381-4bd5-8125-3073647a40de",
          "name": "offers.fares.deeplink.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&destination-name=%7B%7D&encryption-key=%7B%7D&fare=%7B%7D&fare-currency=%7B%7D&lang=%7B%7D&net-fare=%7B%7D&origin=%7B%7D&origin-name=%7B%7D&outbound-segments=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&return-segments=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
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
            "description": "Returns valid deep links for the provided input parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e423ecdc-112f-4f07-8ee0-46f8e5504d72"
            }
          ]
        }
      ]
    },
    {
      "name": "LH",
      "item": [
        {
          "id": "8ae6f41d-344b-430b-8627-230b768d7b91",
          "name": "offers.fares.deeplink.ffp.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink/ffp?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&encryption-key=%7B%7D&lang=%7B%7D&origin=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
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
            "description": "Returns valid LH deep links (FFP - links to flight selection screen on LH.COM)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82a1bcc8-4745-44ae-891f-68275b80c8a5"
            }
          ]
        }
      ]
    }
  ]
}