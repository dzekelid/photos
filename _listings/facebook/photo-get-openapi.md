---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Photo
  description: An individual photo
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{album}/photos:
    get:
      summary: Get Album Photos
      description: The photos contained in this album
      operationId: getAlbumPhotos
      x-api-path-slug: albumphotos-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Photos
    post:
      summary: Post Album Photos
      description: Adds a photo to the album
      operationId: postAlbumPhotos
      x-api-path-slug: albumphotos-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: message
        description: Photo description
      responses:
        200:
          description: OK
      tags:
      - Album
      - Photos
  /{page}/photos:
    get:
      summary: Get Page Photos
      description: The photos contained on this page
      operationId: getPagePhotos
      x-api-path-slug: pagephotos-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
    post:
      summary: Post Page Photos
      description: Adds a photo to the page
      operationId: postPagePhotos
      x-api-path-slug: pagephotos-post
      parameters:
      - in: query
        name: message
        description: Photo description
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
  /{user}/photos:
    get:
      summary: Get User Photos
      description: The photos the user is tagged in
      operationId: getUserPhotos
      x-api-path-slug: userphotos-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Photos
    post:
      summary: Post User Photos
      description: Posts a photo to the user's Wall
      operationId: postUserPhotos
      x-api-path-slug: userphotos-post
      parameters:
      - in: query
        name: message
        description: Photo description
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Photos
  /{photo}:
    get:
      summary: Get Photo
      description: An individual photo
      operationId: getPhoto
      x-api-path-slug: photo-get
      parameters:
      - in: path
        name: photo
        description: Represents the ID of the photo object
      responses:
        200:
          description: OK
      tags:
      - Photo
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