{
  "info": {
    "name": "Sales Force Desk API Create Interaction",
    "_postman_id": "9f8ef98d-4fe5-4cc8-b23c-826ac2601b97",
    "description": "Create interaction.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Interactions",
      "item": [
        {
          "id": "d80d5d8d-15d2-46b7-bea8-ba7c6eb6214b",
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
              "id": "74894b93-2db5-4bc8-b9a0-d14216a81f17"
            }
          ]
        },
        {
          "id": "a38b4e44-8032-4911-9ea4-81734cdda3de",
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
              "id": "7619df8a-1fe0-463d-9493-3e7d85a15fca"
            }
          ]
        }
      ]
    }
  ]
}