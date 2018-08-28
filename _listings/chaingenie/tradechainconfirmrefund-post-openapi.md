---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Refund buyer and stop trade (by Seller)
  description: "Seller can cancel the market trade after bid/buy by refunding the
    seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow
    from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd
    transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tradechain/ConfirmRefund:
    post:
      summary: Refund buyer and stop trade (by Seller)
      description: "Seller can cancel the market trade after bid/buy by refunding
        the seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow
        from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd
        transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
      operationId: TradechainConfirmRefundPost
      x-api-path-slug: tradechainconfirmrefund-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      - in: formData
        name: itemSellerName
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Refund
      - Buyer
      - Stop
      - Trade
      - (by
      - Seller)
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