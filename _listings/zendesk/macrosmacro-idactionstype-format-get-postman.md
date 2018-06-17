{
  "info": {
    "name": "Sales Force Desk API Get Macro Action",
    "_postman_id": "345fbccf-ef8e-4a34-8d77-e31fa7a6b78c",
    "description": "Get macro action.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Interactions",
      "item": [
        {
          "id": "70c4594a-cdea-4529-b89c-31fe48a936d9",
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
              "id": "ab1c372d-d4bb-43ac-b5ca-3771923291f3"
            }
          ]
        },
        {
          "id": "c3c1ac5b-0a0f-4f99-8854-7797e6e3ee51",
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
              "id": "487c6764-84d9-4496-9ce0-ccfd44bbc6de"
            }
          ]
        }
      ]
    },
    {
      "name": "Macros",
      "item": [
        {
          "id": "44f501a7-57ec-4336-885d-3af73206c073",
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
              "id": "663254ff-8177-4300-9255-d48075d7f838"
            }
          ]
        },
        {
          "id": "1041f42b-8f5b-4f22-9e84-a5012abe1cd8",
          "name": "get-macro-action",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "macros/:macro_id/actions/:type.json"
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
                },
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get macro action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3883564-e052-4fb9-b2f2-2b1adbf39886"
            }
          ]
        }
      ]
    }
  ]
}