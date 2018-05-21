{
  "info": {
    "name": "AWS Elastic MapReduce API List Bootstrap Actions",
    "_postman_id": "04a29b9b-e0b4-4d3b-8db1-e4e43b368606",
    "description": "Provides information about the bootstrap actions associated with a cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bootstrap Actions",
      "item": [
        {
          "id": "53e4647b-66cb-4690-857d-bb9f735dc035",
          "name": "listBootstrapActions",
          "request": {
            "url": "http://example.com/api/?Action=ListBootstrapActions?ClusterId=ClusterId&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the bootstrap actions associated with a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8274e5d-fd7f-44a6-87e9-c1377f4e26a4"
            }
          ]
        }
      ]
    }
  ]
}