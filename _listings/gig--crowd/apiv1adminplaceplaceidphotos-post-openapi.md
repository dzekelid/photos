---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Admin Place Placeid Photos
  version: 1.0.0
  description: Post admin place placeid photos.
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