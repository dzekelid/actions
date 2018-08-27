---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API List Actions
  version: 1.0.0
  description: List of all Actions.
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
  /v1/actions/:action:
    get:
      summary: Get action
      description: Gets a single action type
      operationId: get-action
      x-api-path-slug: v1actionsaction-get
      parameters:
      - in: query
        name: |-
          action
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
  ? |2-

        /api/{version}/actions
  : ? |2-

          get
    : summary: Get Actions (Alerts) List
      description: Returns a list of actions (alerts) that have been generated for
        your account.
      operationId: get-actions-alerts-list
      x-api-path-slug: apiversionactions-get
      parameters:
      - in: query
        name: checkids
        description: Comma-separated list of check identifiers
        type: <td>string</td>
      - in: query
        name: contactids
        description: Comma-separated list of contact identifiers
        type: <td>string</td>
      - in: query
        name: from
        description: Only include actions generated later than this timestamp
        type: <td>integer</td>
      - in: query
        name: limit
        description: Limits the number of returned results to the specified quantity
        type: <td>integer (max 300)</td>
      - in: query
        name: offset
        description: Offset for listing
        type: <td>integer</td>
      - in: query
        name: status
        description: Comma-separated list of statuses
        type: <td>string (sent, delivered, error, not_deliv
      - in: query
        name: to
        description: Only include actions generated prior to this timestamp
        type: <td>integer</td>
      - in: query
        name: via
        description: Comma-separated list of via mediums
        type: <td>string (email, sms, twitter, iphone, andr
      responses:
        200:
          description: OK
      tags:
      - Actions
  /actions:
    post:
      summary: Create Action
      description: Create a new Action.
      operationId: create-action
      x-api-path-slug: actions-post
      parameters:
      - in: path
        name: "action_name\n        \n        \n            required\n            Display
          name for the Action.\n        \n    \n    \n        \n        action_url\n
          \       \n        \n            required\n            URL to be invoked
          for action execution."
      responses:
        200:
          description: OK
      tags:
      - Actions
    get:
      summary: List Actions
      description: List of all Actions.
      operationId: list-actions
      x-api-path-slug: actions-get
      parameters:
      - in: path
        name: "maintenance_id\n        \n        \n            string\n            Unique
          ID generated by the server. This can be used as an identifier.\n        \n
          \               \n    \n        \n        display_name\n        \n        \n
          \           string\n            Displa"
      responses:
        200:
          description: OK
      tags:
      - Actions
  /actions/{action_id}:
    put:
      summary: Update Action
      description: Update an existing Action.
      operationId: update-action
      x-api-path-slug: actionsaction-id-put
      parameters:
      - in: path
        name: "action_name\n        \n        \n            required\n            Display
          name for the Action.\n        \n    \n    \n        \n        action_url\n
          \       \n        \n            required\n            URL to be invoked
          for action execution."
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