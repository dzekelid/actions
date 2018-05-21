---
name: Square
x-slug: square
description: Starting with a free credit card reader for the iPhone, iPad, and Android
  devices, Square Reader allows anyone to accept credit cards anywhere, anytime, for
  a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square Register
  serves as a full point-of-sale system for businesses to accept payments, manage
  items, and share menu and location information. Square Wallet, available in the
  US, is the most seamless way to pay, enabling individuals to pay at their favorite
  local businesses, discover new ones nearby, explore menu listings, and store receipts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Actions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Get V2 Locations Location Transactions
  x-api-slug: square-connect-api
  description: |-
    Lists transactions for a particular location.

    Transactions include payment information from sales and exchanges and refund
    information from returns and exchanges.

    Max results per [page](#paginatingresults): 50
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions
  tags: Locations,Location,Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactions-get-openapi.md
- name: Square Connect API Post V2 Locations Location Transactions
  x-api-slug: square-connect-api
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions
  tags: Locations,Location,Transactions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactions-post-openapi.md
- name: Square Connect API Get V2 Locations Location Transactions Transaction
  x-api-slug: square-connect-api
  description: Get v2 locations location transactions transaction.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions/{transaction_id}
  tags: Locations,Location,Transactions,Transaction
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-id-get-openapi.md
- name: Square Connect API Post V2 Locations Location Transactions Transaction Capture
  x-api-slug: square-connect-api
  description: |-
    Captures a transaction that was created with the [Charge](#endpoint-charge)
    endpoint with a `delay_capture` value of `true`.

    See [Delayed capture transactions](/articles/delayed-capture-transactions/)
    for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions/{transaction_id}/capture
  tags: Locations,Location,Transactions,Transaction,Capture
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-idcapture-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-idcapture-post-openapi.md
- name: Square Connect API Post V2 Locations Location Transactions Transaction Refund
  x-api-slug: square-connect-api
  description: |-
    Initiates a refund for a previously charged tender.

    You must issue a refund within 120 days of the associated payment. See
    [this article](https://squareup.com/help/us/en/article/5060) for more information
    on refund behavior.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions/{transaction_id}/refund
  tags: Locations,Location,Transactions,Transaction,Refund
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-idrefund-post-openapi.md
- name: Square Connect API Post V2 Locations Location Transactions Transaction Vo
  x-api-slug: square-connect-api
  description: |-
    Cancels a transaction that was created with the [Charge](#endpoint-charge)
    endpoint with a `delay_capture` value of `true`.

    See [Delayed capture transactions](/articles/delayed-capture-transactions/)
    for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1///v2/locations/{location_id}/transactions/{transaction_id}/void
  tags: Locations,Location,Transactions,Transaction,Void
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-idvoid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/v2locationslocation-idtransactionstransaction-idvoid-post-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Starting with a free credit card reader for the iPhone, iPad, and Android
    devices, Square Reader allows anyone to accept credit cards anywhere, anytime,
    for a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square
    Register serves as a full point-of-sale system for businesses to accept payments,
    manage items, and share menu and location information. Square Wallet, available
    in the US, is the most seamless way to pay, enabling individuals to pay at their
    favorite local businesses, discover new ones nearby, explore menu listings, and
    store receipts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1/
  tags: Actions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---