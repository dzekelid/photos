swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
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
  /photos/{PHOTO_ID}:
    get:
      summary: Get Photos Photo
      description: /updates/marknotificationsread
      operationId: updatesmarknotificationsread
      x-api-path-slug: photosphoto-id-get
      parameters:
      - in: query
        name: PHOTO_ID
        description: The ID of the photo to retrieve additional information for
      - in: path
        name: PHOTO_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Photo
  /users/{USER_ID}/photos:
    get:
      summary: Get Users Photos
      description: /users/{USER_ID}/mayorships
      operationId: usersuser-idmayorships
      x-api-path-slug: usersuser-idphotos-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: USER_ID
        description: Identity of the user to get details for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Photos
  /venues/{VENUE_ID}/photos:
    get:
      summary: Get Venues Photos
      description: /venues/{VENUE_ID}/menu
      operationId: venuesvenue-idmenu
      x-api-path-slug: venuesvenue-idphotos-get
      parameters:
      - in: query
        name: group
        description: Pass checkin for photos added by friends on their recent checkins
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: The venue you want photos for
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Photos