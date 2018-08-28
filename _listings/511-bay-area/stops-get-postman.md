{
  "info": {
    "name": "Bay Area 511 Transit API Stops API",
    "_postman_id": "6f0f81d9-7e00-4b82-9c90-6315e7cdaf58",
    "description": "San francisco 511 transit stops api.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "511",
      "item": [
        {
          "id": "d9d873ae-9f96-4bc7-95c7-c3ee842c0ace",
          "name": "LinesGet",
          "request": {
            "url": "http://api.511.org/transit/lines?api_key=%7B%7D&operator_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit lines api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8837ad2f-9439-44ab-b29c-4a3eda21ac62"
            }
          ]
        },
        {
          "id": "f24a0a9b-77c4-4aa3-a33c-77a4e4f27a36",
          "name": "PatternsGet",
          "request": {
            "url": "http://api.511.org/transit/patterns?api_key=%7B%7D&operator_id=%7B%7D&pattern_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit transit patterns api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4edb4b0f-bf3e-4430-8edc-f010e407a583"
            }
          ]
        },
        {
          "id": "1fb1539e-4bac-4977-addd-b0f3d9437b6c",
          "name": "StopsGet",
          "request": {
            "url": "http://api.511.org/transit/stops?api_key=%7B%7D&operator_id=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "San francisco 511 transit stops api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e39657c-bf28-450d-93ac-65f22cfe8f77"
            }
          ]
        }
      ]
    }
  ]
}