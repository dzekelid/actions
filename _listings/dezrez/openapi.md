swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/globalsearch/auctions:
    get:
      summary: Search for Actions across the system.
      description: Search for actions across the system..
      operationId: GlobalSearch_AuctionsBydataContract.termBydataContract.pageSizeBydataContract.pageNumberBydataContra
      x-api-path-slug: apiglobalsearchauctions-get
      parameters:
      - in: query
        name: dataContract.branchId
      - in: query
        name: dataContract.excludeArchived
      - in: query
        name: dataContract.excludeDeleted
      - in: query
        name: dataContract.groupTypes
      - in: query
        name: dataContract.lastUpdated
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.serviceType
      - in: query
        name: dataContract.term
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - SearchActions
      - Across
      - System