---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API List Bootstrap Actions
  version: 1.0.0
  description: Provides information about the bootstrap actions associated with a
    cluster.
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