---
name: New Relic
x-slug: new-relic
description: New Relic offers SaaS Software Analytics Platform that offers Application
  Performance Management and Real User Monitoring for Cloud and Data Center deployed
  web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
  also offers mobile monitoring solutions for iOS and Android applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
x-kinRank: "8"
x-alexaRank: ""
tags: Actions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Key Transactions. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a paginated \nlist of the key transactions
    associated with your New Relic account.  The time range for summary data is the
    last 10 minutes.\n\nKey transactions can be filtered by their name or list of
    IDs.\n\nSee our documentation for a discussion of \nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///key_transactions.{format}
  tags: Key, Transactions., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/key-transactionsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/key-transactionsformat-get-openapi.md
- name: New Relic Get Key Transactions  . Format
  x-api-slug: new-relic
  description: "This endpoint returns a single key transaction, identified by ID.
    The time range for summary data is the last 10 minutes.\n\nSee our documentation
    for a discussion of \nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///key_transactions/{id}.{format}
  tags: Key, Transactions, , ., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/key-transactionsidformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/key-transactionsidformat-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic offers SaaS Software Analytics Platform that offers Application
    Performance Management and Real User Monitoring for Cloud and Data Center deployed
    web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
    also offers mobile monitoring solutions for iOS and Android applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Actions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---