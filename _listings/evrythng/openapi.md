---
swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 1
info:
  title: EVRYTHNG
  description: the-evrythng-platform-is-a-cloud-platformasaservice-paas-for-storing-sharing-and-analyzing-data-generated-by-physical-objects--the-platform-gives-a-unique-and-permanent-digital-identity-also-known-as-adis-to-each-individual-object-and-allows-authorized-applications-and-users-to-access-it-via-rest-and-pubsub-mqtt-apis--visualisations-in-the-evrythng-dashboard-analytics-conditional-redirections-and-the-reactor-rules-engine-provide-means-to-add-intelligent-behavior-and-features-on-top-of-your-data-to-add-value-
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
  /actions:
    get:
      summary: /actions?project={id} (O)
      description: '**OPERATOR** returns all the action types in the scope of an Application.'
      operationId: ActionsGet2
      x-api-path-slug: actions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: project
      responses:
        200:
          description: OK
      tags:
      - Actions
    post:
      summary: /actions?project={id} (O)
      description: '**OPERATOR** creates a new custom action type for app ID (visible
        only by that app).'
      operationId: ActionsPost2
      x-api-path-slug: actions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: project
      responses:
        200:
          description: OK
      tags:
      - Actions
---