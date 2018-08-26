{
  "info": {
    "name": "Standard Chartered Retrieve trade finance customer profile",
    "_postman_id": "95e66a25-b33e-4085-a503-1edc731fb271",
    "description": "Retrieve trade finance customer profile",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "2a86b8ac-e0c8-444b-af05-64779f88b7ae",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/account"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetAccountBalance??? API upon successful user authentication and entitlement checks will return the various types of ???Account Balances??? applicable for the specified Account Number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79a12ee9-35ba-427f-b7b7-d9160435d298"
            }
          ]
        },
        {
          "id": "88113378-a403-455e-80b6-f62c5fbd17c5",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewTransactionRequestTypes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/transaction-request-types"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetTransactionTypes??? API upon successful user authentication and entitlement checks will return the supported transaction types for the specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "602534ce-2332-4599-8e90-72ec8cc0ec2c"
            }
          ]
        },
        {
          "id": "f248d67a-2eb0-4853-8329-ecdeaf119ebb",
          "name": "getCibServiceS2bApiV1BanksScbAccountsViewAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:viewId/accounts"
              ],
              "variable": [
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List available bank accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4993b79-b49a-44f3-b7dc-7ff9118ebc8c"
            }
          ]
        },
        {
          "id": "a6cc52b6-de51-4254-9276-6024159cc340",
          "name": "postCibServiceS2bApiV1BanksScbReferenceDefaultBranches",
          "request": {
            "url": "http://developer.sc.com/cib/service/s2b/api/v1/banks/scb/reference/default/branches",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetBankCode??? API returns list of Bank Codes for the specified combination of ???Country???, ???City??? and ???Bank??? combination. The data will contain the ???Bank Code(s)??? as well as the address for the Bank & Branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c611688-cd68-46d1-9875-62fc6bed5667"
            }
          ]
        },
        {
          "id": "11c552a2-7779-4c89-9230-e0265ea99b0a",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCountryCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/country/:country"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Country</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "394be8b2-2c4c-4395-927b-0d6b96419120"
            }
          ]
        },
        {
          "id": "b5350afe-f6b4-4af3-84c2-b4ec683fdd03",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCurrencyCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/currency/:currency"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Currency</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4819f656-9289-47fd-af67-b8163221c15f"
            }
          ]
        },
        {
          "id": "b09f536f-4fe3-49ee-83ad-7d7b015aab9c",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerProfile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/profile"
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
            "description": "Retrieve trade finance customer profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1058ecc-cba3-4707-a848-133ff1a6fd4e"
            }
          ]
        }
      ]
    }
  ]
}