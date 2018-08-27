swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeEnvironmentManagedActions:
    get:
      summary: Describe Environment Managed Actions
      description: Lists an environment's upcoming and in-progress managed actions.
      operationId: describeEnvironmentManagedActions
      x-api-path-slug: actiondescribeenvironmentmanagedactions-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      - in: query
        name: Status
        description: To show only actions with a particular status, specify a status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments