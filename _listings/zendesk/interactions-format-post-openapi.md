---
swagger: "2.0"
x-collection-name: Zendesk
x-complete: 0
info:
  title: Sales Force Desk API Create Interaction
  description: Create interaction.
  version: v2
host: yoursite.desk.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /interactions.{format}:
    get:
      summary: Get Interactions
      description: Get interactions.
      operationId: get-interactions
      x-api-path-slug: interactions-format-get
      parameters:
      - in: path
        name: format
      responses:
        200:
          description: OK
      tags:
      - Interactions
      - Format
    post:
      summary: Create Interaction
      description: Create interaction.
      operationId: create-interaction
      x-api-path-slug: interactions-format-post
      parameters:
      - in: path
        name: format
      responses:
        200:
          description: OK
      tags:
      - Interactions
      - Format
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