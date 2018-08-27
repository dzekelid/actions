swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 1
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListBootstrapActions:
    get:
      summary: List Bootstrap Actions
      description: Provides information about the bootstrap actions associated with
        a cluster.
      operationId: listBootstrapActions
      x-api-path-slug: actionlistbootstrapactions-get
      parameters:
      - in: query
        name: ClusterId
        description: The cluster identifier for the bootstrap actions to list
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bootstrap Actions