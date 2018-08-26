---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/History/limit/trades:
    get:
      summary: Get API History Limit Trades
      description: Get api history limit trades.
      operationId: ApiHistoryLimitTradesGet
      x-api-path-slug: apihistorylimittrades-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - History
      - Limit
      - Trades
  /api/BcnTransaction/offchain-trade:
    get:
      summary: Get API Bcntransaction Offchain Trade
      description: Get api bcntransaction offchain trade.
      operationId: ApiBcnTransactionOffchain-tradeGet
      x-api-path-slug: apibcntransactionoffchaintrade-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransaction
      - Offchain
      - Trade
  /api/Ethereum/trade:
    post:
      summary: Add API Ethereum Trade
      description: Add api ethereum trade.
      operationId: ApiEthereumTradePost
      x-api-path-slug: apiethereumtrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Trade
  /api/offchain/trade:
    post:
      summary: Add API Offchain Trade
      description: Add api offchain trade.
      operationId: ApiOffchainTradePost
      x-api-path-slug: apioffchaintrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Trade
  /api/offchain/limit/trade:
    post:
      summary: Add API Offchain Limit Trade
      description: Add api offchain limit trade.
      operationId: ApiOffchainLimitTradePost
      x-api-path-slug: apioffchainlimittrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - Trade
---