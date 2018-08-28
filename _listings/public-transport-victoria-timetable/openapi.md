swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 1
info:
  title: Public Transport Victoria Timetable
  description: the-ptv-timetable-api-provides-direct-access-to-public-transport-victorias-public-transport-timetable-data--the-api-returns-scheduled-timetable-route-and-stop-data-for-all-metropolitan-and-regional-train-tram-and-bus-services-in-victoria-including-night-networknight-train-and-night-tram-data-are-included-in-metropolitan-train-and-tram-services-data-respectively-whereas-night-bus-is-a-separate-route-type--the-api-also-returns-realtime-data-for-metropolitan-train-tram-and-bus-services-where-this-data-is-made-available-to-ptv-as-well-as-disruption-information-stop-facility-information-and-access-to-myki-ticket-outlet-data-
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
  /v3/stops/{stop_id}/route_type/{route_type}:
    get:
      summary: Get V3 Stops Stop Route Type Route Type
      description: View facilities at a specific stop (metro and v/line stations only).
      operationId: Stops_StopDetails
      x-api-path-slug: v3stopsstop-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: gtfs
        description: Incdicates whether the stop_id is a GTFS ID or not
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: stop_accessibility
        description: Indicates if stop accessibility information will be returned
          (default = false)
      - in: query
        name: stop_amenities
        description: Indicates if stop amenity information will be returned (default
          = false)
      - in: query
        name: stop_contact
        description: Placeholder for future development; currently unavailable
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: stop_location
        description: Indicates if stop location information will be returned (default
          = false)
      - in: query
        name: stop_ticket
        description: Placeholder for future development; currently unavailable
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Stop
      - Id
      - Route
      - Type
      - Route
      - Type