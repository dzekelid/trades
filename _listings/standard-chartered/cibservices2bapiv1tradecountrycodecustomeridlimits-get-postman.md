{
  "info": {
    "name": "Standard Chartered Retrieve trade finance limit details",
    "_postman_id": "da4654c4-14fb-4dbc-99a2-bf394a70b68c",
    "description": "Retrieve trade finance limit details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "342477d3-0363-4f84-8bd4-2464051c87a5",
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
              "id": "46825008-d43c-407e-8a44-d0850c1f43e5"
            }
          ]
        },
        {
          "id": "3521a53e-bc0a-4959-8aa5-49d256660177",
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
              "id": "b1506046-7bdc-48a4-8682-233f30a12645"
            }
          ]
        },
        {
          "id": "6d0c69a5-7b55-49f1-b632-ac5bb8784aa5",
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
              "id": "858c84d3-623c-46ae-934a-3f11fa11c215"
            }
          ]
        },
        {
          "id": "7c88e37f-b036-43c3-8a81-86529ab2403d",
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
              "id": "6153ab62-bf5a-4878-928d-8e37181baf0e"
            }
          ]
        },
        {
          "id": "60337c9c-18db-45c6-ba69-a5e8f3522ea7",
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
              "id": "4a706ba4-4ef6-4caf-bc58-aa3af4d7bfad"
            }
          ]
        },
        {
          "id": "d5ed1149-6f42-49da-bb76-f7d06a0490c5",
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
              "id": "ab25c455-4e41-4049-b981-b9f819ff2fb7"
            }
          ]
        },
        {
          "id": "f471765d-bb5d-4df1-8a07-290550c931c1",
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
              "id": "2afbef03-135e-48f9-a4b2-09a6265e5fff"
            }
          ]
        },
        {
          "id": "45e998d9-3cb0-4f5f-a4b6-356e69f73eb0",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerLimits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/limits"
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
            "description": "Retrieve trade finance limit details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "027df0ba-66e3-46df-a846-27ea297db414"
            }
          ]
        }
      ]
    }
  ]
}