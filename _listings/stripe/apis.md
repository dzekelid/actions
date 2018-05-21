---
name: Stripe
x-slug: stripe
description: 'Stripe is a simple, developer-friendly way to accept payments online.
  They believe that enabling transactions on the web is a problem rooted in code,
  not finance, and they want to help put more websites in business. '
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
x-kinRank: "10"
x-alexaRank: ""
tags: Actions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Get Bitcoin Receivers Receiver Transactions
  x-api-slug: stripe
  description: Get Bitcoin, Receivers, Receiver, Transactions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///bitcoin/receivers/{receiver}/transactions
  tags: Bitcoin, Receivers, Receiver, Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/bitcoinreceiversreceivertransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/bitcoinreceiversreceivertransactions-get-openapi.md
- name: Stripe Get Bitcoin Transactions
  x-api-slug: stripe
  description: Get Bitcoin, Transactions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///bitcoin/transactions
  tags: Bitcoin, Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/bitcointransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/bitcointransactions-get-openapi.md
- name: Stripe Get Sources Source Source Transactions
  x-api-slug: stripe
  description: Get Sources, Source, Source, Transactions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/source_transactions
  tags: Sources, Source, Source, Transactions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/sourcessourcesource-transactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/sourcessourcesource-transactions-get-openapi.md
- name: Stripe Get Sources Source Source Transactions Source Transaction
  x-api-slug: stripe
  description: Retrieve an existing source transaction object. Supply the unique source
    ID from a source creation request and the source transaction ID and Stripe will
    return the corresponding up-to-date source object information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///sources/{source}/source_transactions/{source_transaction}
  tags: Sources, Source, Source, Transactions, Source, Transaction
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/sourcessourcesource-transactionssource-transaction-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/sourcessourcesource-transactionssource-transaction-get-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/stripe-black.png
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Actions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/stripe/openapi.md
x-common:
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-github
  url: https://github.com/stripe
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---