{
  "info": {
    "name": "Standard Chartered Retrieve all trade finance transaction status for the current date (localised to tz)",
    "_postman_id": "d5411e13-9abf-4bdf-84c6-a90405cbaafa",
    "description": "Retrieve all trade finance transaction status for the current date (localised to tz)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "c1720924-e7bf-4ee1-8ab4-2067bb931684",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/transactions"
              ],
              "query": [
                {
                  "key": "tz",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all trade finance transaction status for the current date (localised to tz)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fee56a9f-6366-4c0f-99d0-7d6b681dc612"
            }
          ]
        }
      ]
    }
  ]
}