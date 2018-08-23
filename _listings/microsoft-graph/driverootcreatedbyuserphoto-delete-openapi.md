---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Delete Photo
  description: Delete photo Delete a photo.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id | userPrincipalName}/photo:
    delete:
      summary: Delete Photo
      description: Delete photo Delete a photo.
      operationId: DeletePhoto
      x-api-path-slug: usersid--userprincipalnamephoto-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current tag on the item, a 412 Precondition Failed response
          is returned and the item will not be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
  /groups/{id}/photo:
    delete:
      summary: Delete Photo
      description: Delete photo Delete a photo.
      operationId: DeletePhoto
      x-api-path-slug: groupsidphoto-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current tag on the item, a 412 Precondition Failed response
          is returned and the item will not be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
  /drive/root/createdByUser/photo:
    delete:
      summary: Delete Photo
      description: Delete photo Delete a photo.
      operationId: DeletePhoto
      x-api-path-slug: driverootcreatedbyuserphoto-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: if-match
        description: If this request header is included and the eTag (or cTag) provided
          does not match the current tag on the item, a 412 Precondition Failed response
          is returned and the item will not be deleted
        type: string
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