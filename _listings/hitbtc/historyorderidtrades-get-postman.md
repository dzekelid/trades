{
  "info": {
    "name": "HitBTC Get Historical Trades By Specified Order",
    "_postman_id": "837f4276-3f75-4107-93bd-7ea47de8d869",
    "description": "Get historical trades by specified order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "51d18bec-0633-45f0-8642-4ec9627c4da4",
          "name": "getHistoryTrades",
          "request": {
            "url": "{{default}}/history/trades?by=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort=%7B%7D&symbol=%7B%7D&till=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical trades."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1669829d-0922-4e39-975b-c8aa1b0dc0a3"
            }
          ]
        },
        {
          "id": "03061e28-2d99-4363-835d-be57a1a27087",
          "name": "getHistoryOrder",
          "request": {
            "url": "{{default}}/history/order?clientOrderId=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&symbol=%7B%7D&till=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d3bd4bc-9557-4805-8a81-9309cdb8750f"
            }
          ]
        },
        {
          "id": "c751890f-0eb3-4f3a-8806-6bc46724934f",
          "name": "getHistoryOrderTrades",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "history/order/:id/trades"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical trades by specified order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c60cc0b-b597-49da-9998-b046b8da00d9"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api/2"
    }
  ]
}