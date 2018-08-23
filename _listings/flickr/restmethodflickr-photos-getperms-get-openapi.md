---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Photos Get Perms
  description: Get permissions for a photo.
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
  /rest/?method=flickr.photos.addTags:
    post:
      summary: Photos Add Tags
      description: Add tags to a photo.
      operationId: postRestMethodFlickr.photos.addtags
      x-api-path-slug: restmethodflickr-photos-addtags-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to add tags to
      - in: query
        name: tags
        description: The tags to add to the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - AddTags
  /rest/?method=flickr.photos.delete:
    post:
      summary: Photos Delete
      description: Delete a photo from Flickr.
      operationId: postRestMethodFlickr.photos.delete
      x-api-path-slug: restmethodflickr-photos-delete-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to delete
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Delete
  /rest/?method=flickr.photos.getAllContexts:
    get:
      summary: Photos Get All Contexts
      description: Returns all visible sets and pools the photo belongs to.
      operationId: getRestMethodFlickr.photos.getallcontexts
      x-api-path-slug: restmethodflickr-photos-getallcontexts-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The photo to return information for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetAllContexts
  /rest/?method=flickr.photos.getContactsPhotos:
    get:
      summary: Photos Get Contacts Photos
      description: Fetch a list of recent photos from the calling users' contacts.
      operationId: getRestMethodFlickr.photos.getcontactsphotos
      x-api-path-slug: restmethodflickr-photos-getcontactsphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: count
        description: Number of photos to return
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: include_self
        description: Set to 1 to include photos from the calling user
      - in: query
        name: just_friends
        description: Set as 1 to only show photos from friends and family (excluding
          regular contacts)
      - in: query
        name: single_photo
        description: Only fetch one photo (the latest) per contact, instead of all
          photos in chronological order
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetContactsPhotos
  /rest/?method=flickr.photos.getContactsPublicPhotos:
    get:
      summary: Photos Get Contacts Public Photos
      description: Fetch a list of recent public photos from a users' contacts.
      operationId: getRestMethodFlickr.photos.getcontactspublicphotos
      x-api-path-slug: restmethodflickr-photos-getcontactspublicphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: count
        description: Number of photos to return
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: include_self
        description: Set to 1 to include photos from the calling user
      - in: query
        name: just_friends
        description: Set as 1 to only show photos from friends and family (excluding
          regular contacts)
      - in: query
        name: single_photo
        description: Only fetch one photo (the latest) per contact, instead of all
          photos in chronological order
      - in: query
        name: user_id
        description: The NSID of the user to fetch photos for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetContactsPublicPhotos
  /rest/?method=flickr.photos.getContext:
    get:
      summary: Photos Get Context
      description: Returns next and previous photos for a photo in a photostream.
      operationId: getRestMethodFlickr.photos.getcontext
      x-api-path-slug: restmethodflickr-photos-getcontext-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to fetch the context for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetContext
  /rest/?method=flickr.photos.getCounts:
    get:
      summary: Photos Get Counts
      description: Returns next and previous photos for a photo in a photostream.
      operationId: getRestMethodFlickr.photos.getcounts
      x-api-path-slug: restmethodflickr-photos-getcounts-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: dates
        description: A comma delimited list of unix timestamps, denoting the periods
          to return counts for
      - in: query
        name: format
        description: Response format
      - in: query
        name: taken_dates
        description: A comma delimited list of mysql datetimes, denoting the periods
          to return counts for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetCounts
  /rest/?method=flickr.photos.getExif:
    get:
      summary: Photos Get Exif
      description: Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling
        user must have permission to view the photo.
      operationId: getRestMethodFlickr.photos.getexif
      x-api-path-slug: restmethodflickr-photos-getexif-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to fetch information for
      - in: query
        name: secret
        description: The secret for the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetExif
  /rest/?method=flickr.photos.getFavorites:
    get:
      summary: Photos Get Favorites
      description: Returns the list of people who have favorited a given photo.
      operationId: getRestMethodFlickr.photos.getfavorites
      x-api-path-slug: restmethodflickr-photos-getfavorites-get
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
        description: Number of users to return per page
      - in: query
        name: photo_id
        description: The id of the photo to fetch the favoriters list for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetFavorites
  /rest/?method=flickr.photos.getInfo:
    get:
      summary: Photos Get Info
      description: Get information about a photo. The calling user must have permission
        to view the photo.
      operationId: getRestMethodFlickr.photos.getinfo
      x-api-path-slug: restmethodflickr-photos-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to get information for
      - in: query
        name: secret
        description: The secret for the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetInfo
  /rest/?method=flickr.photos.getNotInSet:
    get:
      summary: Photos Get Not In Set
      description: Returns a list of your photos that are not part of any sets.
      operationId: getRestMethodFlickr.photos.getnotinset
      x-api-path-slug: restmethodflickr-photos-getnotinset-get
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
        name: max_taken_date
        description: Maximum taken date
      - in: query
        name: max_upload_date
        description: Maximum upload date
      - in: query
        name: media
        description: Filter results by media type
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
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetNotInSet
  /rest/?method=flickr.photos.getPerms:
    get:
      summary: Photos Get Perms
      description: Get permissions for a photo.
      operationId: getRestMethodFlickr.photos.getperms
      x-api-path-slug: restmethodflickr-photos-getperms-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to get permissions for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetPerms
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