---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Uninstall action
  version: 1.0.0
  description: Uninstalls an action and remove it from the associated alarms(s).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/actions:
    get:
      summary: Get all available action types
      description: Gets all known action types
      operationId: get-all-available-action-types
      x-api-path-slug: v1actions-get
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed:
    get:
      summary: Get all installed actions
      description: Gets all actions that are installed for the project
      operationId: get-all-installed-actions
      x-api-path-slug: v1actionsinstalled-get
      responses:
        200:
          description: OK
      tags:
      - Actions
    put:
      summary: Install action
      description: Installs an action
      operationId: install-action
      x-api-path-slug: v1actionsinstalled-put
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId:
    get:
      summary: Get details of an installed action
      description: Gets a single action definition
      operationId: get-details-of-an-installed-action
      x-api-path-slug: v1actionsinstalledactionid-get
      parameters:
      - in: query
        name: |-
          actionId
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
    delete:
      summary: Uninstall action
      description: Uninstalls an action and remove it from the associated alarms(s).
      operationId: uninstall-action
      x-api-path-slug: v1actionsinstalledactionid-delete
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId/alarms:
    get:
      summary: Get all alarms using an action
      description: Get alarms that are using this action installed for the project
      operationId: get-all-alarms-using-an-action
      x-api-path-slug: v1actionsinstalledactionidalarms-get
      responses:
        200:
          description: OK
      tags:
      - Actions
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