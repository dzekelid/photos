---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Photos Add
  description: /photos/{PHOTO_ID}
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos/add:
    post:
      summary: Post Photos Add
      description: /photos/{PHOTO_ID}
      operationId: photosphoto-id
      x-api-path-slug: photosadd-post
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Vertical accuracy of the users location, in meters
      - in: query
        name: broadcast
        description: Whether to broadcast this photo
      - in: query
        name: checkinId
        description: The ID of a checkin owned by the user
      - in: query
        name: Content-Type
        description: Content-Type
      - in: query
        name: image
        description: The image file data
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: llAcc
        description: Accuracy of the users latitude and longitude, in meters
      - in: query
        name: public
        description: When the checkinId is also provided (meaning this is a photo
          attached to a checkin), this parameter allows for making the photo public
          and viewable at the venue
      - in: query
        name: tipId
        description: The ID of a tip owned by the user
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: The ID of a venue, provided only when adding a public photo of
          the venue in general, rather than a private checkin or tip photo using the
          parameters above
      responses:
        200:
          description: OK
      tags:
      - Photos
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