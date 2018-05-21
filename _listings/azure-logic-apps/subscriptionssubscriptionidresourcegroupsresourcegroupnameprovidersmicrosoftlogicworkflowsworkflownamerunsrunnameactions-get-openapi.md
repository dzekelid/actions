---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Workflow Run Actions List
  description: Gets a list of workflow run actions.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/workflows/{workflowName}/runs/{runName}/actions
  : get:
      summary: Workflow Run Actions List
      description: Gets a list of workflow run actions.
      operationId: WorkflowRunActions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftlogicworkflowsworkflownamerunsrunnameactions-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      - in: path
        name: runName
        description: The workflow run name
      - in: path
        name: workflowName
        description: The workflow name
      responses:
        200:
          description: OK
      tags:
      - Workflow Run Actions
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