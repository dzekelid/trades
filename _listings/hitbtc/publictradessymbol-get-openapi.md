---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Trades
  description: Trades.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /public/trades/{symbol}:
    get:
      summary: Trades
      description: Trades.
      operationId: getPublicTradesSymbol
      x-api-path-slug: publictradessymbol-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: from
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: path
        name: symbol
      - in: query
        name: till
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      responses:
        200:
          description: OK
      tags:
      - Trades
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---