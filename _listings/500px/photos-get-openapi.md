---
swagger: "2.0"
x-collection-name: 500px
x-complete: 0
info:
  title: 500px Get Photos
  description: Returns a listing of twenty (up to one hundred) photos for a specified
    photo stream.
  version: v1
host: api.500px.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos:
    get:
      summary: Get Photos
      description: Returns a listing of twenty (up to one hundred) photos for a specified
        photo stream.
      operationId: getPhotos
      x-api-path-slug: photos-get
      parameters:
      - in: query
        name: exclude
        description: String name of the category to exclude photos by
      - in: query
        name: feature
        description: Photo stream to be retrieved
      - in: query
        name: image_size
        description: The photo size to be returned
      - in: query
        name: include_states
        description: If set to 1, returns state of the photo for the currently logged
          in user and authenticated request
      - in: query
        name: include_store
        description: If set to 1, returns market infomation about the photo
      - in: query
        name: only
        description: String name of the category to return photos from
      - in: query
        name: page
        description: Return a specific page in the photo stream
      - in: query
        name: rpp
        description: The number of results to return
      - in: query
        name: sort
        description: Sort photos in the specified order
      - in: query
        name: sort_direction
        description: Control the order of the sorting
      - in: query
        name: tags
        description: If set to 1, returns an array of tags for the photo
      - in: query
        name: username
        description: OR username for user Photo streeam
      - in: query
        name: user_id
        description: User ID user Photo streeam
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