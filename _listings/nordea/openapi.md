---
swagger: "2.0"
x-collection-name: Nordea
x-complete: 1
info:
  title: Nordea
  description: the-nordeas-open-banking-initiative-obi-api-offers-a-safe-and-simple-way-to-try-out-the-upcoming-obi-this-api-is-a-sandbox-version-and-its-purpose-is-to-make-developers-familiar-with-the-upcoming-obi-production-release-moreover-it-allows-the-developers-to-experiment-and-build-applications-which-use-the-obi-before-its-official-release-
  contact:
    name: Open Banking team
  version: 1.0.0
host: api.nordeaopenbanking.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/transactions:
    get:
      summary: Get account transactions
      description: Get accounts account transactions
      operationId: transactionsList
      x-api-path-slug: accountsaccountidtransactions-get
      parameters:
      - in: path
        name: accountId
        description: Internal account identifier
      - in: query
        name: continuationKey
        description: Resource listing may return a continuationKey if theres more
          results available
      - in: query
        name: fromDate
        description: List transactions starting from and including this date
      - in: query
        name: language
        description: Preferred language for textual values
      - in: query
        name: toDate
        description: List transactions until and including this date
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Account
      - Transactions
---