{
  "info": {
    "name": "Sales Force Desk API Get Macro Actions",
    "_postman_id": "95f920d6-15af-492e-a056-775e7c0ee499",
    "description": "Get macro actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Interactions",
      "item": [
        {
          "id": "80e0bf6f-1fa8-4a9f-97af-6a7bf86dd354",
          "name": "get-interactions",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/interactions.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get interactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce686e43-d0d9-4079-9b95-f0a4cb5f9831"
            }
          ]
        },
        {
          "id": "8d31e192-48eb-4b02-a86d-84084b339491",
          "name": "create-interaction",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/interactions.json?format=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create interaction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "349e6551-8bc9-4e4b-8da4-623e472872cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Macros",
      "item": [
        {
          "id": "e243840f-3164-4e06-9b6e-ce2163f6a58b",
          "name": "get-macro-actions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "macros/:macro_id/actions.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "macro_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get macro actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "006b04d9-41db-4395-a931-ae697dc40be7"
            }
          ]
        }
      ]
    }
  ]
}