---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 0
info:
  title: EVRYTHNG /actions/scans (U)
  description: |-
    **USER** creates a "scan" action on a thng.

    **ATTENTION -->** use a valid thng ID in the payload!
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /actions/scans:
    post:
      summary: /actions/scans (U)
      description: |-
        **USER** creates a "scan" action on a thng.

        **ATTENTION -->** use a valid thng ID in the payload!
      operationId: ActionsScansPost2
      x-api-path-slug: actionsscans-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Actions
      - Scans
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