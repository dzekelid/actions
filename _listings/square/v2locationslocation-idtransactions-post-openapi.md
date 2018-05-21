---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Post V2 Locations Location Transactions
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