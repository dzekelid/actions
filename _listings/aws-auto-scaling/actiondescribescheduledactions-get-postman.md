{
  "info": {
    "name": "AWS Auto Scaling API Describe Scheduled Actions",
    "_postman_id": "3180e819-dfd7-4150-92d4-9b380441a508",
    "description": "Describes the actions scheduled for your Auto Scaling group that haven't run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Scheduled Actions",
      "item": [
        {
          "id": "676ad314-d795-46ec-b838-66260c4660f7",
          "name": "describeScheduledActions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScheduledActions?AutoScalingGroupName=AutoScalingGroupName&EndTime=EndTime&MaxRecords=MaxRecords&NextToken=NextToken&ScheduledActionNames.member.N=ScheduledActionNames.member.N&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the actions scheduled for your Auto Scaling group that haven't run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0089b6c3-5e64-488b-9a9a-9454af19cff3"
            }
          ]
        }
      ]
    }
  ]
}