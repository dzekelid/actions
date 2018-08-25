---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePendingMaintenanceActions:
    get:
      summary: Describe Pending Maintenance Actions
      description: Returns a list of resources (for example, DB instances) that have
        at least one pending maintenance action.
      operationId: describependingmaintenanceactions
      x-api-path-slug: actiondescribependingmaintenanceactions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more resources to return pending
          maintenance actions for
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribePendingMaintenanceActions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ResourceIdentifier
        description: The ARN of a resource to return pending maintenance actions for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance Actions
---