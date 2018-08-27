swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeScheduledActions:
    get:
      summary: Describe Scheduled Actions
      description: Describes the actions scheduled for your Auto Scaling group that
        haven't run.
      operationId: describeScheduledActions
      x-api-path-slug: actiondescribescheduledactions-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: EndTime
        description: The latest scheduled start time to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ScheduledActionNames.member.N
        description: Describes one or more scheduled actions
        type: string
      - in: query
        name: StartTime
        description: The earliest scheduled start time to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Actions