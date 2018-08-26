---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/transactions/{transaction_id}/complete:
    post:
      summary: Complete request money
      description: Lets the recipient of a money request complete the request by sending
        money to the user who requested the money. This can only be completed by the
        user to whom the request was made, not the user who sent the request.
      operationId: lets-the-recipient-of-a-money-request-complete-the-request-by-sending-money-to-the-user-who-requeste
      x-api-path-slug: accountsaccount-idtransactionstransaction-idcomplete-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Complete
      - Request
      - Money
---