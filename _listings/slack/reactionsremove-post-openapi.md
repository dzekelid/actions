---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Remove Reaction
  description: Removes a reaction from an item.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reactions.list:
    get:
      summary: List Reactions
      description: Lists reactions made by a user.
      operationId: reactions_list
      x-api-path-slug: reactionslist-get
      parameters:
      - in: query
        name: count
      - in: query
        name: full
        description: If true always return the complete reaction list
      - in: query
        name: page
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: user
        description: Show reactions made by this user
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Messaging
      - Reactions
  /reactions.add:
    post:
      summary: Add Reaction
      description: Adds a reaction to an item.
      operationId: reactions_add
      x-api-path-slug: reactionsadd-post
      parameters:
      - in: formData
        name: channel
        description: Channel where the message to add reaction to was posted
      - in: formData
        name: file
        description: File to add reaction to
      - in: formData
        name: file_comment
        description: File comment to add reaction to
      - in: formData
        name: name
        description: Reaction (emoji) name
      - in: formData
        name: timestamp
        description: Timestamp of the message to add reaction to
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Reactions
  /reactions.get:
    get:
      summary: Get Reaction
      description: Gets reactions for an item.
      operationId: reactions_get
      x-api-path-slug: reactionsget-get
      parameters:
      - in: query
        name: channel
        description: Channel where the message to get reactions for was posted
      - in: query
        name: file
        description: File to get reactions for
      - in: query
        name: file_comment
        description: File comment to get reactions for
      - in: query
        name: full
        description: If true always return the complete reaction list
      - in: query
        name: timestamp
        description: Timestamp of the message to get reactions for
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Reactions
  /reactions.remove:
    post:
      summary: Remove Reaction
      description: Removes a reaction from an item.
      operationId: reactions_remove
      x-api-path-slug: reactionsremove-post
      parameters:
      - in: formData
        name: channel
        description: Channel where the message to remove reaction from was posted
      - in: formData
        name: file
        description: File to remove reaction from
      - in: formData
        name: file_comment
        description: File comment to remove reaction from
      - in: formData
        name: name
        description: Reaction (emoji) name
      - in: formData
        name: timestamp
        description: Timestamp of the message to remove reaction from
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Reactions
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