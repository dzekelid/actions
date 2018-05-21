---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user-admin/v1/users:
    get:
      summary: List a Group&#8217;s Users
      description: List a Group&#8217;s Users
      operationId: useradminv1usersgroupidactions
      x-api-path-slug: useradminv1users-get
      parameters:
      - in: query
        name: actions
        description: When enabled, response yields additional details on users&#8217;
          access rights
        type: string
      - in: query
        name: groupId
        description: Unique numeric identifier for a group
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Admin
      - Users
      - Group
      - actions
---