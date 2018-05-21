---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global Historical
  description: ondemand-global-historical-quotes
  version: 1.0.0
host: www.xignite.com
basePath: xGlobalHistorical.json/XigniteGlobalHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAllCorporateActionsByExchange:
    post:
      summary: Get All Corporate Actions By Exchange
      description: Get all corporate actions for a date range in the specified exchange.
      operationId: postGetallcorporateactionsbyexchange
      x-api-path-slug: getallcorporateactionsbyexchange-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Actions
      - By
      - Exchange
---