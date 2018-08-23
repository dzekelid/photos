---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Art Photo Photoid Thumb
  version: 1.0.0
  description: Get art photo photoid thumb.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/place/{placeId}/photos:
    post:
      summary: Post Admin Place Placeid Photos
      description: Post admin place placeid photos.
      operationId: postApiV1AdminPlacePlacePhotos
      x-api-path-slug: apiv1adminplaceplaceidphotos-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Photos
  /api/v1/event/{eventId}/photos:
    post:
      summary: Post Event Eventid Photos
      description: Post event eventid photos.
      operationId: postApiV1EventEventPhotos
      x-api-path-slug: apiv1eventeventidphotos-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photos
  /api/v1/admin/place/{placeId}/photo/{photoId}:
    delete:
      summary: Delete Admin Place Placeid Photo Photoid
      description: Delete admin place placeid photo photoid.
      operationId: deleteApiV1AdminPlacePlacePhotoPhoto
      x-api-path-slug: apiv1adminplaceplaceidphotophotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
      - Photo
      - Photoid
  /api/v1/art/photo/{photoId}:
    get:
      summary: Get Art Photo Photoid
      description: Get art photo photoid.
      operationId: getApiV1ArtPhotoPhoto
      x-api-path-slug: apiv1artphotophotoid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Photoid
  /api/v1/art/photo/{photoId}/thumb:
    get:
      summary: Get Art Photo Photoid Thumb
      description: Get art photo photoid thumb.
      operationId: getApiV1ArtPhotoPhotoThumb
      x-api-path-slug: apiv1artphotophotoidthumb-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Photoid
      - Thumb
  /api/v1/art/photo/{type}:
    post:
      summary: Post Art Photo Type
      description: Post art photo type.
      operationId: postApiV1ArtPhotoType
      x-api-path-slug: apiv1artphototype-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Type
  /api/v1/art/photo/{id}:
    delete:
      summary: Delete Art Photo
      description: Delete art photo.
      operationId: deleteApiV1ArtPhoto
      x-api-path-slug: apiv1artphotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
  /api/v1/event/{eventId}/photo:
    post:
      summary: Post Event Eventid Photo
      description: Post event eventid photo.
      operationId: postApiV1EventEventPhoto
      x-api-path-slug: apiv1eventeventidphoto-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photo
  /api/v1/event/{eventId}/photo/{photoId}:
    delete:
      summary: Delete Event Eventid Photo Photoid
      description: Delete event eventid photo photoid.
      operationId: deleteApiV1EventEventPhotoPhoto
      x-api-path-slug: apiv1eventeventidphotophotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photo
      - Photoid
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