---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Client/pendingActions:
    get:
      summary: Get API Client Pendingactions
      description: Get api client pendingactions.
      operationId: ApiClientPendingActionsGet
      x-api-path-slug: apiclientpendingactions-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Pendingactions
---