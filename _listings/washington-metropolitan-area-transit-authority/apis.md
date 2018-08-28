---
name: Washington Metropolitan Area Transit Authority
x-slug: washington-metropolitan-area-transit-authority
description: Official feed of Metro/WMATA, not monitored 24/7. Report emergencies
  to Transit Police at (202) 962-2121. Service updates @metrorailinfo & @metrobusinfo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
x-kinRank: "8"
x-alexaRank: "24927"
tags: Stops
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/apis.md
specificationVersion: "0.14"
apis:
- name: Bus Route and Stop Methods - JSON - Schedule at Stop
  x-api-slug: jsonjstopschedule-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Bus.svc
  tags: Transit, Transit, Transportation, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/jsonjstopschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/jsonjstopschedule-get-openapi.md
- name: Bus Route and Stop Methods - JSON - Stop Search
  x-api-slug: jsonjstops-get
  description: "Description\r\n\r\nReturns a list of nearby bus stops based on latitude,
    longitude, and radius.\r\nOmit all parameters to retrieve a list of all stops.\r\n\r\nResponse
    Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nStops\r\n\r\n\r\nArray
    containing stop information (Stop).\r\n\r\n\r\n\r\n\r\n\r\n\r\nStop Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
    name. May be slightly different from what is spoken or\r\ndisplayed in the bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString
    array of route variants which provide service at this\r\nstop. Note that these
    are not date-specific; any route variant\r\nwhich stops at this stop on any day
    will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit regional ID which can be
    used in various bus-related\r\nmethods. If unavailable, the StopID will be 0 or
    NULL."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Bus.svc
  tags: Transit, Transit, Transportation, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/jsonjstops-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/jsonjstops-get-openapi.md
- name: Bus Route and Stop Methods - XML - Schedule
  x-api-slug: routeschedule-get
  description: "Description\r\n\r\nReturns schedules for a given route variant for
    a given date.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nDirection0/Direction1\r\n\r\n\r\nArrays
    containing trip information (Trip).\r\n\r\nMost routes will return content in
    both Direction0 and\r\nDirection1 elements, though a few (especially ones which
    run in\r\na loop, such as the U8) will return content only for Direction0\r\nand
    NULL content for Direction1.\r\n\r\n0 or 1 are binary properties. There is no
    specific mapping to\r\ndirection, but a different value for the same route signifies\r\nthat
    the route is in an opposite direction.\r\n\r\n\r\n\r\n\r\nName\r\n\r\nDescriptive
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
    to what is displayed on the\r\nbus.\r\n\r\n\r\n\r\nTripID\r\n\r\nUnique trip ID.
    This can be correlated with the data returned\r\nfrom the schedule-related methods.\r\n\r\n\r\n\r\n\r\n\r\nStopTime
    Elements\r\n\r\n\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit regional ID which can be
    used in various bus-related\r\nmethods. If unavailable, the StopID will be 0 or
    NULL.\r\n\r\n\r\n\r\nStopName\r\n\r\nStop name. May be slightly different from
    what is spoken or\r\ndisplayed in the bus.\r\n\r\n\r\n\r\nStopSeq\r\n\r\nOrder
    of the stop in the sequence of StopTimes.\r\n\r\n\r\n\r\nTime\r\n\r\nScheduled
    departure date and time (Eastern Standard Time) from\r\nthis stop. Will be in
    YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T13:17:00)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Bus.svc
  tags: Transit, Transit, Transportation, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/routeschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/routeschedule-get-openapi.md
- name: Bus Route and Stop Methods - XML - Schedule at Stop
  x-api-slug: stopschedule-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Bus.svc
  tags: Transit, Transit, Transportation, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/stopschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/stopschedule-get-openapi.md
- name: Bus Route and Stop Methods - XML - Stop Search
  x-api-slug: stops-get
  description: "Description\r\n\r\nReturns a list of nearby bus stops based on latitude,
    longitude, and radius.\r\nOmit all parameters to retrieve a list of all stops.\r\n\r\nResponse
    Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nStops\r\n\r\n\r\nArray
    containing stop information (Stop).\r\n\r\n\r\n\r\n\r\n\r\n\r\nStop Elements\r\n\r\n\r\n\r\n\r\n\r\nLat\r\n\r\nLatitude.\r\n\r\n\r\n\r\nLon\r\n\r\nLongitude.\r\n\r\n\r\n\r\nName\r\n\r\nStop
    name. May be slightly different from what is spoken or\r\ndisplayed in the bus.\r\n\r\n\r\n\r\nRoutes\r\n\r\nString
    array of route variants which provide service at this\r\nstop. Note that these
    are not date-specific; any route variant\r\nwhich stops at this stop on any day
    will be listed.\r\n\r\n\r\n\r\nStopID\r\n\r\n7-digit regional ID which can be
    used in various bus-related\r\nmethods. If unavailable, the StopID will be 0 or
    NULL."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1214-washington-metropolitan-area-transit-authority.jpg
  humanURL: http://wmata.com/
  baseURL: https://api.wmata.com//Bus.svc
  tags: Transit, Transit, Transportation, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/stops-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stops/master/_listings/washington-metropolitan-area-transit-authority/stops-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://vzaar.api.gallery.streamdata.io
- type: x-api-stack
  url: http://washington.metropolitan.area.transit.authority.stack.network
- type: x-base
  url: http://api.wmata.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/wmata
- type: x-developer
  url: http://developer.wmata.com/
- type: x-email
  url: boardofdirectors@wmata.com
- type: x-email
  url: metrotransit@wmata.com
- type: x-email
  url: adaassist@wmata.com
- type: x-email
  url: access@wmata.com
- type: x-email
  url: cjachles@wmata.com
- type: x-email
  url: writtentestimony@wmata.com
- type: x-email
  url: speak@wmata.com
- type: x-email
  url: SEBusMove@wmata.com
- type: x-email
  url: PARP@wmata.com
- type: x-email
  url: raccomments@wmata.com
- type: x-signup
  url: https://developer.wmata.com/signup/
- type: x-twitter
  url: https://twitter.com/wmata
- type: x-website
  url: http://wmata.com/
- type: x-website
  url: http://wmata.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---