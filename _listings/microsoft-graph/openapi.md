---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
    get:
      summary: Get Photo
      description: Get photo Retrieve the properties and relationships of photo object.
      operationId: GetPhoto
      x-api-path-slug: usersid--userprincipalnamephoto-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
    patch:
      summary: Update Photo
      description: Update photo Update the properties of photo object.
      operationId: UpdatePhoto
      x-api-path-slug: usersid--userprincipalnamephoto-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
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
    get:
      summary: Get Photo
      description: Get photo Retrieve the properties and relationships of photo object.
      operationId: GetPhoto
      x-api-path-slug: groupsidphoto-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
    patch:
      summary: Update Photo
      description: Update photo Update the properties of photo object.
      operationId: UpdatePhoto
      x-api-path-slug: groupsidphoto-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
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
    get:
      summary: Get Photo
      description: Get photo Retrieve the properties and relationships of photo object.
      operationId: GetPhoto
      x-api-path-slug: driverootcreatedbyuserphoto-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
    patch:
      summary: Update Photo
      description: Update photo Update the properties of photo object.
      operationId: UpdatePhoto
      x-api-path-slug: driverootcreatedbyuserphoto-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Photo
---