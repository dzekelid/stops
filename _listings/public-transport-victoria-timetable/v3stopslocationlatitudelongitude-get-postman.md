{
  "info": {
    "name": "PTV Timetable API - Version 3 Get V3 Stops Location Latitude , Longitude",
    "_postman_id": "67866c31-1c12-4d48-b203-e0ad8905d2ed",
    "description": "View all stops near a specific location.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stops",
      "item": [
        {
          "id": "c03ffbb8-e1b0-4eda-bf44-00d570dc1be5",
          "name": "Stops_StopsByGeolocation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/stops/location/:latitude,:longitude"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_distance",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "route_types",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "latitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "longitude",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all stops near a specific location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92a3eaf5-f946-4a3c-af21-1779dd6f3dd2"
            }
          ]
        }
      ]
    }
  ]
}