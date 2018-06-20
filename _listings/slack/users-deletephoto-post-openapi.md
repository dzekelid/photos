---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Delete Photo
  description: Delete the user profile photo
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users.deletePhoto:
    post:
      summary: Delete Photo
      description: Delete the user profile photo
      operationId: users_deletePhoto
      x-api-path-slug: users-deletephoto-post
      parameters:
      - in: formData
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
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