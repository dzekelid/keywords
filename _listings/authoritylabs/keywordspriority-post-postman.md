{
  "info": {
    "name": "Authority Labs Partner API Priority Queue",
    "_postman_id": "c97533b0-460e-4959-bced-088d3194ac39",
    "description": "Priority Queue",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keywords",
      "item": [
        {
          "id": "cb1d363e-d0a6-46ad-9043-52e024a2879a",
          "name": "delayed-queue",
          "request": {
            "url": "http://api.authoritylabs.com/keywords",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delayed Queue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8b5f861-4302-445a-92da-6723715c6310"
            }
          ]
        },
        {
          "id": "3d6c9e0e-a370-4ea7-855c-af58c24bfb9e",
          "name": "priority-queue",
          "request": {
            "url": "http://api.authoritylabs.com/keywords/priority",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Priority Queue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "054f1fda-3056-4e5f-ab69-ae62b0c57e0d"
            }
          ]
        }
      ]
    }
  ]
}