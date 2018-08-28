swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/profile-picture:
    delete:
      summary: Deletes profile picture by user id
      description: Deletes profile picture by user id.
      operationId: deleteProfilePictureById
      x-api-path-slug: usersuseridprofilepicture-delete
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Picture
      - By
      - User
    post:
      summary: Uploads and sets profile picture by user id
      description: Uploads and sets profile picture by user id.
      operationId: setProfilePictureById
      x-api-path-slug: usersuseridprofilepicture-post
      parameters:
      - in: body
        name: body
        description: Picture
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Sets
      - Profile
      - Picture
      - By
      - User
  /users/by-username/{username}/profile-picture:
    delete:
      summary: Deletes profile picture by username
      description: Deletes profile picture by username.
      operationId: deleteProfilePictureByUsername
      x-api-path-slug: usersbyusernameusernameprofilepicture-delete
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Picture
      - By
      - Username
    post:
      summary: Uploads and sets profile picture by username
      description: Uploads and sets profile picture by username.
      operationId: setProfilePictureByUsername
      x-api-path-slug: usersbyusernameusernameprofilepicture-post
      parameters:
      - in: body
        name: body
        description: Picture
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Sets
      - Profile
      - Picture
      - By
      - Username