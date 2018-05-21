---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Post V2 Locations Location Transactions Transaction Vo
  description: |-
    Cancels a transaction that was created with the [Charge](#endpoint-charge)
    endpoint with a `delay_capture` value of `true`.

    See [Delayed capture transactions](/articles/delayed-capture-transactions/)
    for more information.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: 1.0.0
host: connect.squareup.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/locations/{location_id}/transactions:
    get:
      summary: Get V2 Locations Location Transactions
      description: |-
        Lists transactions for a particular location.

        Transactions include payment information from sales and exchanges and refund
        information from returns and exchanges.

        Max results per [page](#paginatingresults): 50
      operationId: getV2LocationsLocationTransactions
      x-api-path-slug: v2locationslocation-idtransactions-get
      parameters:
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in RFC 3339
          format
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      - in: query
        name: end_time
        description: The end of the requested reporting period, in RFC 3339 format
      - in: path
        name: location_id
        description: The ID of the location to list transactions for
      - in: query
        name: sort_order
        description: The order in which results are listed in the response (`ASC`
          foroldest first, `DESC` for newest first)
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
    post:
      summary: Post V2 Locations Location Transactions
      description: |-
        Charges a card represented by a card nonce or a customer's card on file.

        Your request to this endpoint must include _either_:

        - A value for the `card_nonce` parameter (to charge a card nonce generated
        with the `SqPaymentForm`)
        - Values for the `customer_card_id` and `customer_id` parameters (to charge
        a customer's card on file)

        In order for an eCommerce payment to potentially qualify for
        [Square chargeback protection](https://squareup.com/help/article/5394), you
        _must_ provide values for the following parameters in your request:

        - `buyer_email_address`
        - At least one of `billing_address` or `shipping_address`

        When this response is returned, the amount of Square's processing fee might not yet be
        calculated. To obtain the processing fee, wait about ten seconds and call
        [RetrieveTransaction](#endpoint-retrievetransaction). See the `processing_fee_money`
        field of each [Tender included](#type-tender) in the transaction.
      operationId: postV2LocationsLocationTransactions
      x-api-path-slug: v2locationslocation-idtransactions-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to associate the created transaction with
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
  /v2/locations/{location_id}/transactions/{transaction_id}:
    get:
      summary: Get V2 Locations Location Transactions Transaction
      description: Get v2 locations location transactions transaction.
      operationId: getV2LocationsLocationTransactionsTransaction
      x-api-path-slug: v2locationslocation-idtransactionstransaction-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the transactions associated location
      - in: path
        name: transaction_id
        description: The ID of the transaction to retrieve
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
      - Transaction
  /v2/locations/{location_id}/transactions/{transaction_id}/capture:
    post:
      summary: Post V2 Locations Location Transactions Transaction Capture
      description: |-
        Captures a transaction that was created with the [Charge](#endpoint-charge)
        endpoint with a `delay_capture` value of `true`.

        See [Delayed capture transactions](/articles/delayed-capture-transactions/)
        for more information.
      operationId: postV2LocationsLocationTransactionsTransactionCapture
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idcapture-post
      parameters:
      - in: path
        name: location_id
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
      - Transaction
      - Capture
  /v2/locations/{location_id}/transactions/{transaction_id}/refund:
    post:
      summary: Post V2 Locations Location Transactions Transaction Refund
      description: |-
        Initiates a refund for a previously charged tender.

        You must issue a refund within 120 days of the associated payment. See
        [this article](https://squareup.com/help/us/en/article/5060) for more information
        on refund behavior.
      operationId: postV2LocationsLocationTransactionsTransactionRefund
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idrefund-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the original transactions associated location
      - in: path
        name: transaction_id
        description: The ID of the original transaction that includes the tender to
          refund
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
      - Transaction
      - Refund
  /v2/locations/{location_id}/transactions/{transaction_id}/void:
    post:
      summary: Post V2 Locations Location Transactions Transaction Vo
      description: |-
        Cancels a transaction that was created with the [Charge](#endpoint-charge)
        endpoint with a `delay_capture` value of `true`.

        See [Delayed capture transactions](/articles/delayed-capture-transactions/)
        for more information.
      operationId: postV2LocationsLocationTransactionsTransactionVo
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idvoid-post
      parameters:
      - in: path
        name: location_id
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Location
      - Transactions
      - Transaction
      - Void
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