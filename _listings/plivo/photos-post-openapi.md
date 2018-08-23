---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Photos
  description: Create a new photo on behalf of the user, and receive an upload key
    in exchange.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos:
    post:
      summary: Post Photos
      description: Create a new photo on behalf of the user, and receive an upload
        key in exchange.
      operationId: create-a-new-photo-on-behalf-of-the-user-and-receive-an-upload-key-in-exchange
      x-api-path-slug: photos-post
      parameters:
      - in: query
        name: aperture
        description: Aperture value
      - in: query
        name: camera
        description: Make and model of the camera
      - in: query
        name: category
        description: A numerical ID for the Category of the photo
      - in: query
        name: description
        description: Description for the photo
      - in: query
        name: focal_length
        description: Focal length in millimetres, a string representing an integer
          value
      - in: query
        name: iso
        description: ISO value
      - in: query
        name: latitude
        description: Latitude, in decimal format
      - in: query
        name: lens
        description: Lens used to make this photo
      - in: query
        name: longitude
        description: Longitude, in decimal format
      - in: query
        name: name
        description: Title of the photo
      - in: query
        name: privacy
        description: Whether to hide the photo from the user profile on the website
      - in: query
        name: shutter_speed
        description: Shutter speed in seconds, represented by string containing a
          rational expression if the value is 1sec
      - in: query
        name: tags
        description: Comma-separated list of tags to apply to the photo
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