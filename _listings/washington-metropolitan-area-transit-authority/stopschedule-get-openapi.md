---
swagger: "2.0"
x-collection-name: Washington Metropolitan Area Transit Authority
x-complete: 0
info:
  title: WMATA Bus Route and Stop Methods XML - Schedule at Stop
  description: "Description\r\n\r\nReturns a set of buses scheduled at a stop for
    a given date.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrivals\r\n\r\n\r\nArray
    containing scheduled arrival information (ScheduleArrival).\r\n\r\n\r\n\r\n\r\nStop\r\n\r\n\r\nStructure
    describing stop information.\r\n\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrival Elements\r\n\r\n\r\n\r\n\r\n\r\nDirectionNum\r\n\r\nDenotes
    a binary direction (0 or 1) of the bus. There is no\r\nspecific mapping to direction,
    but a different value for the same\r\nroute signifies that the buses are traveling
    in opposite\r\ndirections. Use the TripDirectionText element to show the actual\r\ndestination
    of the bus.\r\n\r\n\r\n\r\nEndTime\r\n\r\nScheduled end date and time (Eastern
    Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nRouteID\r\n\r\nBus
    route variant identifier (pattern). This variant can be\r\nused in several other
    bus methods which accept variants. Note that\r\ncustomers will never see anything
    other than the base route name,\r\nso variants 10A, 10Av1, 10Av2, etc. will be
    displayed as 10A on the\r\nbus.\r\n\r\n\r\n\r\nScheduleTime\r\n\r\nDate and time
    (Eastern Standard Time) when the bus is scheduled\r\nto stop at this location.
    Will be in YYYY-MM-DDTHH:mm:ss format\r\n(e.g.: 2014-10-27T13:17:00).\r\n\r\n\r\n\r\nStartTime\r\n\r\nScheduled
    start date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
    format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nTripDirectionText\r\n\r\nGeneral
    direction of the trip (e.g.: NORTH, SOUTH, EAST,\r\nWEST).\r\n\r\n\r\n\r\nTripHeadsign\r\n\r\nDestination
    of the bus.\r\n\r\n\r\n\r\nTripID\r\n\r\nTrip identifier. This can be correlated
    with the data in our\r\nbus schedule information as well as bus positions.\r\n\r\n\r\n\r\n\r\n\r\nStop
    Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
    name. May be slightly different from what is spoken or\r\ndisplayed in the bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString
    array of route variants which provide service at this\r\nstop. Note that these
    are not date-specific; any route variant\r\nwhich stops at this stop on any day
    will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit regional ID which can be
    used in various bus-related\r\nmethods. If unavailable, the StopID will be 0 or
    NULL."
  version: 1.0.0
host: api.wmata.com
basePath: /Bus.svc
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /json/jStopSchedule:
    get:
      summary: JSON - Schedule at Stop
      description: "Description\r\n\r\nReturns a set of buses scheduled at a stop
        for a given date.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrivals\r\n\r\n\r\nArray
        containing scheduled arrival information (ScheduleArrival).\r\n\r\n\r\n\r\n\r\nStop\r\n\r\n\r\nStructure
        describing stop information.\r\n\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrival Elements\r\n\r\n\r\n\r\n\r\n\r\nDirectionNum\r\n\r\nDenotes
        a binary direction (0 or 1) of the bus. There is no\r\nspecific mapping to
        direction, but a different value for the same\r\nroute signifies that the
        buses are traveling in opposite\r\ndirections. Use the TripDirectionText element
        to show the actual\r\ndestination of the bus.\r\n\r\n\r\n\r\nEndTime\r\n\r\nScheduled
        end date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nRouteID\r\n\r\nBus route
        variant identifier (pattern). This variant can be\r\nused in several other
        bus methods which accept variants. Note that\r\ncustomers will never see anything
        other than the base route name,\r\nso variants 10A, 10Av1, 10Av2, etc. will
        be displayed as 10A on the\r\nbus.\r\n\r\n\r\n\r\nScheduleTime\r\n\r\nDate
        and time (Eastern Standard Time) when the bus is scheduled\r\nto stop at this
        location. Will be in YYYY-MM-DDTHH:mm:ss format\r\n(e.g.: 2014-10-27T13:17:00).\r\n\r\n\r\n\r\nStartTime\r\n\r\nScheduled
        start date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nTripDirectionText\r\n\r\nGeneral
        direction of the trip (e.g.: NORTH, SOUTH, EAST,\r\nWEST).\r\n\r\n\r\n\r\nTripHeadsign\r\n\r\nDestination
        of the bus.\r\n\r\n\r\n\r\nTripID\r\n\r\nTrip identifier. This can be correlated
        with the data in our\r\nbus schedule information as well as bus positions.\r\n\r\n\r\n\r\n\r\n\r\nStop
        Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
        name. May be slightly different from what is spoken or\r\ndisplayed in the
        bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString array of route variants which provide
        service at this\r\nstop. Note that these are not date-specific; any route
        variant\r\nwhich stops at this stop on any day will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit
        regional ID which can be used in various bus-related\r\nmethods. If unavailable,
        the StopID will be 0 or NULL."
      operationId: 5476362a281d830c946a3d6c
      x-api-path-slug: jsonjstopschedule-get
      parameters:
      - in: query
        name: Date
        description: Date in YYYY-MM-DD format for which to retrieve schedule
      - in: query
        name: StopID
        description: 7-digit regional stop ID
      responses:
        200:
          description: OK
      tags:
      - Buses
      - Stops
      - Schedules
  /json/jStops:
    get:
      summary: JSON - Stop Search
      description: "Description\r\n\r\nReturns a list of nearby bus stops based on
        latitude, longitude, and radius.\r\nOmit all parameters to retrieve a list
        of all stops.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nStops\r\n\r\n\r\nArray
        containing stop information (Stop).\r\n\r\n\r\n\r\n\r\n\r\n\r\nStop Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
        name. May be slightly different from what is spoken or\r\ndisplayed in the
        bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString array of route variants which provide
        service at this\r\nstop. Note that these are not date-specific; any route
        variant\r\nwhich stops at this stop on any day will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit
        regional ID which can be used in various bus-related\r\nmethods. If unavailable,
        the StopID will be 0 or NULL."
      operationId: 5476362a281d830c946a3d6d
      x-api-path-slug: jsonjstops-get
      parameters:
      - in: query
        name: Lat
        description: Center point Latitude, required if Longitude and Radius are specified
      - in: query
        name: Lon
        description: Center point Longitude, required if Latitude and Radius are specified
      - in: query
        name: Radius
        description: Radius (meters) to include in the search area, required if Latitude
          and Longitude are specified
      responses:
        200:
          description: OK
      tags:
      - Buses
      - Stops
  /RouteSchedule:
    get:
      summary: XML - Schedule
      description: "Description\r\n\r\nReturns schedules for a given route variant
        for a given date.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nDirection0/Direction1\r\n\r\n\r\nArrays
        containing trip information (Trip).\r\n\r\nMost routes will return content
        in both Direction0 and\r\nDirection1 elements, though a few (especially ones
        which run in\r\na loop, such as the U8) will return content only for Direction0\r\nand
        NULL content for Direction1.\r\n\r\n0 or 1 are binary properties. There is
        no specific mapping to\r\ndirection, but a different value for the same route
        signifies\r\nthat the route is in an opposite direction.\r\n\r\n\r\n\r\n\r\nName\r\n\r\nDescriptive
        name for the route.\r\n\r\n\r\n\r\n\r\n\r\nTrip Elements\r\n\r\n\r\n\r\n\r\n\r\nDirectionNum\r\n\r\nDeprecated.
        Use the\r\nTripDirectionText element to denote the general direction of the\r\ntrip.\r\n\r\n\r\n\r\nEndTime\r\n\r\nScheduled
        end date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nRouteID\r\n\r\nBus route
        variant. This can be used in several other bus\r\nmethods which accept variants.\r\n\r\n\r\n\r\nStartTime\r\n\r\nScheduled
        start date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nStopTimes\r\n\r\n\r\nArray
        containing location and time information (StopTime).\r\n\r\n\r\n\r\n\r\nTripDirectionText\r\n\r\nGeneral
        direction of the trip (NORTH, SOUTH, EAST, WEST, LOOP,\r\netc.).\r\n\r\n\r\n\r\nTripHeadsign\r\n\r\nDescriptive
        text of where the bus is headed. This is similar,\r\nbut not necessarily identical,
        to what is displayed on the\r\nbus.\r\n\r\n\r\n\r\nTripID\r\n\r\nUnique trip
        ID. This can be correlated with the data returned\r\nfrom the schedule-related
        methods.\r\n\r\n\r\n\r\n\r\n\r\nStopTime Elements\r\n\r\n\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit
        regional ID which can be used in various bus-related\r\nmethods. If unavailable,
        the StopID will be 0 or NULL.\r\n\r\n\r\n\r\nStopName\r\n\r\nStop name. May
        be slightly different from what is spoken or\r\ndisplayed in the bus.\r\n\r\n\r\n\r\nStopSeq\r\n\r\nOrder
        of the stop in the sequence of StopTimes.\r\n\r\n\r\n\r\nTime\r\n\r\nScheduled
        departure date and time (Eastern Standard Time) from\r\nthis stop. Will be
        in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T13:17:00)."
      operationId: 5476362a281d830c946a3d71
      x-api-path-slug: routeschedule-get
      parameters:
      - in: query
        name: Date
        description: Date in YYYY-MM-DD format for which to retrieve schedule
      - in: query
        name: IncludingVariations
        description: Whether or not to include variations
      - in: query
        name: RouteID
        description: Bus route variant, e
      responses:
        200:
          description: OK
      tags:
      - Buses
      - Stops
      - Schedules
  /StopSchedule:
    get:
      summary: XML - Schedule at Stop
      description: "Description\r\n\r\nReturns a set of buses scheduled at a stop
        for a given date.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrivals\r\n\r\n\r\nArray
        containing scheduled arrival information (ScheduleArrival).\r\n\r\n\r\n\r\n\r\nStop\r\n\r\n\r\nStructure
        describing stop information.\r\n\r\n\r\n\r\n\r\n\r\n\r\nScheduleArrival Elements\r\n\r\n\r\n\r\n\r\n\r\nDirectionNum\r\n\r\nDenotes
        a binary direction (0 or 1) of the bus. There is no\r\nspecific mapping to
        direction, but a different value for the same\r\nroute signifies that the
        buses are traveling in opposite\r\ndirections. Use the TripDirectionText element
        to show the actual\r\ndestination of the bus.\r\n\r\n\r\n\r\nEndTime\r\n\r\nScheduled
        end date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nRouteID\r\n\r\nBus route
        variant identifier (pattern). This variant can be\r\nused in several other
        bus methods which accept variants. Note that\r\ncustomers will never see anything
        other than the base route name,\r\nso variants 10A, 10Av1, 10Av2, etc. will
        be displayed as 10A on the\r\nbus.\r\n\r\n\r\n\r\nScheduleTime\r\n\r\nDate
        and time (Eastern Standard Time) when the bus is scheduled\r\nto stop at this
        location. Will be in YYYY-MM-DDTHH:mm:ss format\r\n(e.g.: 2014-10-27T13:17:00).\r\n\r\n\r\n\r\nStartTime\r\n\r\nScheduled
        start date and time (Eastern Standard Time) for this\r\ntrip. Will be in YYYY-MM-DDTHH:mm:ss
        format (e.g.:\r\n2014-10-27T13:17:00).\r\n\r\n\r\n\r\nTripDirectionText\r\n\r\nGeneral
        direction of the trip (e.g.: NORTH, SOUTH, EAST,\r\nWEST).\r\n\r\n\r\n\r\nTripHeadsign\r\n\r\nDestination
        of the bus.\r\n\r\n\r\n\r\nTripID\r\n\r\nTrip identifier. This can be correlated
        with the data in our\r\nbus schedule information as well as bus positions.\r\n\r\n\r\n\r\n\r\n\r\nStop
        Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
        name. May be slightly different from what is spoken or\r\ndisplayed in the
        bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString array of route variants which provide
        service at this\r\nstop. Note that these are not date-specific; any route
        variant\r\nwhich stops at this stop on any day will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit
        regional ID which can be used in various bus-related\r\nmethods. If unavailable,
        the StopID will be 0 or NULL."
      operationId: 5476362a281d830c946a3d72
      x-api-path-slug: stopschedule-get
      parameters:
      - in: query
        name: Date
        description: Date in YYYY-MM-DD format for which to retrieve schedule
      - in: query
        name: StopID
        description: 7-digit regional stop ID
      responses:
        200:
          description: OK
      tags:
      - Buses
      - Stops
      - Schedules
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