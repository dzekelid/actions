swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/actions.json:
    get:
      summary: List actions
      description: |-
        Fetches multiple action records. The records can be filtered, paged, and sorted according to
        the respective parameters. Only actions that are currently "in_progess" will be returned by
        this endpoint.
      operationId: v2.actions.json.get
      x-api-path-slug: v2actions-json-get
      parameters:
      - in: query
        name: due_on
        description: Equality filters that are applied to the due_on field
      - in: query
        name: ids
        description: IDs of actions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: step_id
        description: Fetch actions by step ID
      - in: query
        name: type
        description: Filter actions by type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Actions