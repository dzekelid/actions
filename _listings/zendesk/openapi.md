---
swagger: "2.0"
x-collection-name: Zendesk
x-complete: 1
info:
  title: Sales Force Desk API
  description: build-deep-integrations-expose-your-service-to-influential-smb-customers-or-just-make-desk-com-work-the-way-you-want-
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
  /macros/{macro_id}/actions.{format}:
    get:
      summary: Get Macro Actions
      description: Get macro actions.
      operationId: get-macro-actions
      x-api-path-slug: macrosmacro-idactions-format-get
      parameters:
      - in: path
        name: format
      - in: path
        name: macro_id
      responses:
        200:
          description: OK
      tags:
      - Macros
      - Macro
      - Actions
      - Format
  /macros/{macro_id}/actions/{type}.{format}:
    get:
      summary: Get Macro Action
      description: Get macro action.
      operationId: get-macro-action
      x-api-path-slug: macrosmacro-idactionstype-format-get
      parameters:
      - in: path
        name: format
      - in: path
        name: macro_id
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Macros
      - Macro
      - Actions
      - Type
      - Format
    put:
      summary: Update Macro Action
      description: Update macro action.
      operationId: update-macro-action
      x-api-path-slug: macrosmacro-idactionstype-format-put
      parameters:
      - in: path
        name: format
      - in: path
        name: macro_id
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Macros
      - Macro
      - Actions
      - Type
      - Format
---