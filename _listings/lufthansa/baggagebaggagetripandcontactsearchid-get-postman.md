{
  "info": {
    "name": "LH Partner Baggage Trip and Contact",
    "_postman_id": "ec816af1-25d1-46bd-9e4e-8c25e3bf3073",
    "description": "Retrieve passenger trip, contact and baggage details. This service is only accessible for LH privileged partners",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baggage",
      "item": [
        {
          "id": "33ae929b-3f3c-4400-a4bf-deeb04446c98",
          "name": "baggage.baggagetripandcontact.searchID.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "baggage/baggagetripandcontact/:searchID"
              ],
              "variable": [
                {
                  "id": "searchID",
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
            "description": "Retrieve passenger trip, contact and baggage details. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46df5cc3-45d1-4b1e-ae8a-014b59b17c43"
            }
          ]
        }
      ]
    }
  ]
}