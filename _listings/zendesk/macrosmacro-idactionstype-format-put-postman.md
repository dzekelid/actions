{
  "info": {
    "name": "Sales Force Desk API Update Macro Action",
    "_postman_id": "de695596-5e6b-4f28-a2b6-204f61f58694",
    "description": "Update macro action.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Interactions",
      "item": [
        {
          "id": "8373f4b4-70e0-415c-af1e-8c3b0d0f34a1",
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
              "id": "3ef81404-31d6-45bb-bac9-d7e0f29f602a"
            }
          ]
        },
        {
          "id": "943b44ff-92e2-4c09-b421-8dcc82ba3982",
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
              "id": "ead5dc83-79f6-40cc-acc0-8e442ed8d7c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Macros",
      "item": [
        {
          "id": "f0cc6658-1e20-4e55-8f20-f9fe5eaabbcb",
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
              "id": "33217890-4157-43ab-8d9e-e7699c156c5b"
            }
          ]
        },
        {
          "id": "aa755236-f213-4054-9a95-e7e2de79c4d7",
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
              "id": "c16b93cb-f13f-41c9-8cc1-e1070c7048b5"
            }
          ]
        },
        {
          "id": "3ccffb6f-d532-49dc-9b62-dc04e3cf440e",
          "name": "update-macro-action",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update macro action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "524f626e-24a9-4da1-b024-d9d4daf569ea"
            }
          ]
        }
      ]
    }
  ]
}