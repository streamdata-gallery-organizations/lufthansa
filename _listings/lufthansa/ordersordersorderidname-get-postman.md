{
  "info": {
    "name": "LH Partner Orders",
    "_postman_id": "b902ace5-840c-4a3d-87db-41bc7cb64c29",
    "description": "Retrieve order by ID and optionally name. This service is only accessible for LH privileged partners",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Orders",
      "item": [
        {
          "id": "4fabe3ee-74de-4398-8fda-0f89b74de8dc",
          "name": "Orders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "orders/orders/:orderID/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "orderID",
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
            "description": "Retrieve order by ID and optionally name. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "960b15a4-6a98-40ef-8517-c912fe6059ef"
            }
          ]
        }
      ]
    }
  ]
}