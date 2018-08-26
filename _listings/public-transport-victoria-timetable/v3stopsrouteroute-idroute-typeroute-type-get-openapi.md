---
swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 0
info:
  title: PTV Timetable API - Version 3 Get V3 Stops Route Route Route Type Route Type
  description: View all stops on a specific route.
  termsOfService: http://ptv.vic.gov.au/ptv-timetable-api/
  contact:
    name: Public Transport Victoria
    url: http://ptv.vic.gov.au/digital
  version: v3
host: timetableapi.ptv.vic.gov.au
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/stops/location/{latitude},{longitude}:
    get:
      summary: Get V3 Stops Location Latitude , Longitude
      description: View all stops near a specific location.
      operationId: Stops_StopsByGeolocation
      x-api-path-slug: v3stopslocationlatitudelongitude-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: latitude
        description: Geographic coordinate of latitude
      - in: path
        name: longitude
        description: Geographic coordinate of longitude
      - in: query
        name: max_distance
        description: Filter by maximum distance (in metres) from location specified
          via latitude and longitude parameters (default = 300)
      - in: query
        name: max_results
        description: Maximum number of results returned (default = 30)
      - in: query
        name: route_types
        description: Filter by route_type; values returned via RouteTypes API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Location
      - Latitude
      - Longitude
  /v3/stops/route/{route_id}/route_type/{route_type}:
    get:
      summary: Get V3 Stops Route Route Route Type Route Type
      description: View all stops on a specific route.
      operationId: Stops_StopsForRoute
      x-api-path-slug: v3stopsrouteroute-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Route
      - Route
      - Id
      - Route
      - Type
      - Route
      - Type
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---