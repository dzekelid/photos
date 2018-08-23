---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr People Get Photos Of
  description: Returns a list of photos containing a particular Flickr member.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.activity.userPhotos:
    get:
      summary: Activity User Photos
      description: Returns a list of recent activity on photos commented on by the
        calling user. Do not poll this method more than once an hour.
      operationId: getRestMethodFlickr.activity.userphotos
      x-api-path-slug: restmethodflickr-activity-userphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of items to return per page
      - in: query
        name: timeframe
        description: The timeframe in which to return updates for
      responses:
        200:
          description: OK
      tags:
      - Activity
      - UserPhotos
  /rest/?method=flickr.galleries.editPhotos:
    post:
      summary: Galleries Edit Photos
      description: Modify the photos in a gallery. Use this method to add, remove
        and re-order photos.
      operationId: postRestMethodFlickr.galleries.editphotos
      x-api-path-slug: restmethodflickr-galleries-editphotos-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: gallery_id
        description: The id of the gallery to modify
      - in: query
        name: photo_ids
        description: A comma-delimited list of photo ids to include in the gallery
      - in: query
        name: primary_photo_id
        description: The id of the photo to use as the primary photo for the gallery
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - EditPhotos
  /rest/?method=flickr.galleries.getPhotos:
    get:
      summary: Galleries Get Photos
      description: Return the list of photos for a gallery.
      operationId: getRestMethodFlickr.galleries.getphotos
      x-api-path-slug: restmethodflickr-galleries-getphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: gallery_id
        description: The ID of the gallery of photos to return
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of galleries to return per page
      responses:
        200:
          description: OK
      tags:
      - Galleries
      - GetPhotos
  /rest/?method=flickr.groups.pools.getPhotos:
    get:
      summary: Groups Pools Get Photos
      description: Returns a list of pool photos for a given group, based on the permissions
        of the group and the user logged in (if any).
      operationId: getRestMethodFlickr.groups.pools.getphotos
      x-api-path-slug: restmethodflickr-groups-pools-getphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: tags
        description: A tag to filter the pool with
      - in: query
        name: user_id
        description: The nsid of a user
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - GetPhotos
  /rest/?method=flickr.panda.getPhotos:
    get:
      summary: Panda Get Photos
      description: Ask the Flickr Pandas for a list of recent public (and "safe")
        photos. More information about the pandas can be found on the dev blog.
      operationId: getRestMethodFlickr.panda.getphotos
      x-api-path-slug: restmethodflickr-panda-getphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: panda_name
        description: The name of the panda to ask for photos from
      - in: query
        name: per_page
        description: Number of photos to return per page
      responses:
        200:
          description: OK
      tags:
      - Panda
      - GetPhotos
  /rest/?method=flickr.people.getPhotos:
    get:
      summary: People Get Photos
      description: Return photos from the given user's photostream. Only photos visible
        to the calling user will be returned. This method must be authenticated; to
        return public photos for a user, use flickr.people.getPublicPhotos.
      operationId: getRestMethodFlickr.people.getphotos
      x-api-path-slug: restmethodflickr-people-getphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: content_type
        description: Content type setting
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_taken_date
        description: Maximum taken date
      - in: query
        name: max_upload_date
        description: Maximum upload date
      - in: query
        name: min_taken_date
        description: Minimum taken date
      - in: query
        name: min_upload_date
        description: Minimum upload date
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: privacy_filter
        description: Return photos only matching a certain privacy level
      - in: query
        name: safe_search
        description: Safe search setting
      - in: query
        name: user_id
        description: The NSID of the user whose photos to return
      responses:
        200:
          description: OK
      tags:
      - People
      - GetPhotos
  /rest/?method=flickr.people.getPhotosOf:
    get:
      summary: People Get Photos Of
      description: Returns a list of photos containing a particular Flickr member.
      operationId: getRestMethodFlickr.people.getphotosof
      x-api-path-slug: restmethodflickr-people-getphotosof-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: owner_id
        description: An NSID of a Flickr member
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: user_id
        description: The NSID of the user you want to find photos of
      responses:
        200:
          description: OK
      tags:
      - People
      - GetPhotosOf
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