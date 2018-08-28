{
  "info": {
    "name": "PTV Timetable API - Version 3 Get V3 Stops Route Route Route Type Route Type",
    "_postman_id": "e5f8ee96-5656-4006-80fe-91a1f2f63fe2",
    "description": "View all stops on a specific route.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Departures",
      "item": [
        {
          "id": "084bff29-d1ae-40df-bd11-ce9ea20a2a3f",
          "name": "Departures_GetForStop",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "platform_numbers",
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
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for all routes from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9532f0de-a213-4969-ab12-7293d8360b41"
            }
          ]
        },
        {
          "id": "2ce13f3f-9ec1-4cfb-99c8-d188ca509c7d",
          "name": "Departures_GetForStopAndRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id/route/:route_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for a specific route from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51e9e74d-3ecf-4b0a-aa14-8223c7676e42"
            }
          ]
        }
      ]
    },
    {
      "name": "Directions",
      "item": [
        {
          "id": "2a2c9b62-0b32-4e6e-831e-f8f7b6341bce",
          "name": "Directions_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View directions that a route travels in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52d79bfa-dd4b-4eb9-a2f9-cd5a9d85dc49"
            }
          ]
        },
        {
          "id": "db47e63a-f8ed-4039-acad-7af035fa38c0",
          "name": "Directions_ForDirection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcf44627-553e-4aca-a6a1-a38b0f4c7cd2"
            }
          ]
        },
        {
          "id": "faec19ed-c13d-4e0c-b97b-6f4c99019106",
          "name": "Directions_ForDirectionAndType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes of a particular type for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e04ab53-689c-424b-944a-4d660267c536"
            }
          ]
        }
      ]
    },
    {
      "name": "Disruptions",
      "item": [
        {
          "id": "107834b0-4964-4d1a-a7cf-b0c302da8403",
          "name": "Disruptions_GetAllDisruptions",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/disruptions?devid=%7B%7D&disruption_status=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for all route types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7391cf5-36e0-4811-98b1-ee8ee3a4137f"
            }
          ]
        },
        {
          "id": "b3df8444-2f3e-4c7f-8163-909df1a7acd8",
          "name": "Disruptions_GetDisruptionsByRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "disruption_status",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for a particular route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5080b05e-4338-4a46-b129-4e20acfd9c9b"
            }
          ]
        },
        {
          "id": "eed7cb56-42ca-42bf-b87f-41dedbb0630e",
          "name": "Disruptions_GetDisruptionById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/:disruption_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "disruption_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View a specific disruption."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23859fe5-3147-49b5-8bbb-910ccf97fa10"
            }
          ]
        }
      ]
    },
    {
      "name": "Pattern",
      "item": [
        {
          "id": "ac754756-a187-4907-a801-a1bea39f247a",
          "name": "Patterns_GetPatternByRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/pattern/run/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stop_id",
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
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the stopping pattern for a specific trip/service run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b0c5881-e71a-4888-bb9b-74b490a82c5e"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "1f23e189-27a5-49bc-af1b-b7d73a86a30e",
          "name": "RouteTypes_GetRouteTypes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/route_types?devid=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all route types and their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6f558fc-b444-4d1a-a7c7-3bf3ff0d66a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "87b8177b-5db5-4e47-b2b7-815909f2e657",
          "name": "Routes_OneOrMoreRoutes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/routes?devid=%7B%7D&route_name=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route names and numbers for all routes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb9f30a1-dd3c-41e2-a3ba-0777059fdb3a"
            }
          ]
        },
        {
          "id": "98b577a7-ba48-4644-a862-b68dd83c5c2d",
          "name": "Routes_RouteFromId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/routes/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route name and number for specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f38c4eb-9821-4960-b7b8-dfd6b0f901d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "4190feac-0c40-4efd-8664-2ff939c62665",
          "name": "Runs_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ac26155-e284-48a9-b093-2a5c975b8dfd"
            }
          ]
        },
        {
          "id": "bf390849-55fa-4bb5-a60e-e60ed0de202f",
          "name": "Runs_ForRouteAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "128fad0d-77d7-4fac-bfed-6cb9dad604f9"
            }
          ]
        },
        {
          "id": "2e30d20c-93df-44d7-92b3-4ae32b34853d",
          "name": "Runs_ForRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific run id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d66af01d-bf6b-4a78-9105-646aa7c31856"
            }
          ]
        },
        {
          "id": "ec1319a1-3cc5-4221-8780-e8506f4eea8a",
          "name": "Runs_ForRunAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the trip/service run for a specific run id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41a98e8e-d79c-4248-90a5-e1ded4d4e704"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "1d427334-dab1-4ffe-aca5-364c09e47b57",
          "name": "Search_Search",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/search/:search_term"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_addresses",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_outlets",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "latitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "longitude",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_distance",
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
                  "id": "search_term",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View stops, routes and myki ticket outlets that match the search term."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b494494-9276-481f-b4f0-60f544d9fcc0"
            }
          ]
        }
      ]
    },
    {
      "name": "Stops",
      "item": [
        {
          "id": "02ddd681-170b-4e6f-b550-fbf6ddfbb27f",
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
              "id": "9161c59e-cc55-475d-9d60-5aa6d2b2d94a"
            }
          ]
        },
        {
          "id": "f2d160b0-c811-49cd-b315-b8159dd92a68",
          "name": "Stops_StopsForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/stops/route/:route_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
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
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all stops on a specific route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f33ae7df-f874-4d42-905e-b1c04b78494f"
            }
          ]
        }
      ]
    }
  ]
}