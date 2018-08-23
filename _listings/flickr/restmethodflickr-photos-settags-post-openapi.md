---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Photos Set Tags
  description: Set the tags for a photo.
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
  /rest/?method=flickr.photos.getRecent:
    get:
      summary: Photos Get Recent
      description: Returns the list of people who have favorited a given photo.
      operationId: getRestMethodFlickr.photos.getrecent
      x-api-path-slug: restmethodflickr-photos-getrecent-get
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
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetRecent
  /rest/?method=flickr.photos.getSizes:
    get:
      summary: Photos Get Sizes
      description: Returns the available sizes for a photo. The calling user must
        have permission to view the photo.
      operationId: getRestMethodFlickr.photos.getsizes
      x-api-path-slug: restmethodflickr-photos-getsizes-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to fetch size information for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetSizes
  /rest/?method=flickr.photos.getUntagged:
    get:
      summary: Photos Get Untagged
      description: Returns a list of your photos that are not tagged.
      operationId: getRestMethodFlickr.photos.getuntagged
      x-api-path-slug: restmethodflickr-photos-getuntagged-get
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
      - GetUntagged
  /rest/?method=flickr.photos.getWithGeoData:
    get:
      summary: Photos Get With Geo Data
      description: Returns a list of your geo-tagged photos.
      operationId: getRestMethodFlickr.photos.getwithgeodata
      x-api-path-slug: restmethodflickr-photos-getwithgeodata-get
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
      - GetWithGeoData
  /rest/?method=flickr.photos.getWithoutGeoData:
    get:
      summary: Photos Get Without Geo Data
      description: Returns a list of your photos which haven't been geo-tagged.
      operationId: getRestMethodFlickr.photos.getwithoutgeodata
      x-api-path-slug: restmethodflickr-photos-getwithoutgeodata-get
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
      - GetWithoutGeoData
  /rest/?method=flickr.photos.getRecentlyUpdated:
    get:
      summary: Photos Get Recently Updated
      description: Return a list of your photos that have been recently created or
        which have been recently modified. Recently modified may mean that the photo's
        metadata (title, description, tags) may have been changed or a comment has
        been added (or just modified somehow :-)
      operationId: getRestMethodFlickr.photos.getrecentlyupdated
      x-api-path-slug: restmethodflickr-photos-getrecentlyupdated-get
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
        name: min_date
        description: A Unix timestamp or any English textual datetime description
          indicating the date from which modifications should be compared
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetRecentlyd
  /rest/?method=flickr.photos.removeTag:
    post:
      summary: Photos Remove Tag
      description: Remove a tag from a photo.
      operationId: postRestMethodFlickr.photos.removetag
      x-api-path-slug: restmethodflickr-photos-removetag-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to add tags to
      - in: query
        name: tag_id
        description: The tag to remove from the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - RemoveTag
  /rest/?method=flickr.photos.search:
    get:
      summary: Photos Search
      description: Return a list of photos matching some criteria. Only photos visible
        to the calling user will be returned. To return private or semi-private photos,
        the caller must be authenticated with 'read' permissions, and have permission
        to view the photos. Unauthenticated calls will only return public photos.
      operationId: getRestMethodFlickr.photos.search
      x-api-path-slug: restmethodflickr-photos-search-get
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: contacts
        description: Search your contacts
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
        name: geo_context
        description: Geo context is a numeric value representing the photos geotagginess
          beyond latitude and longitude
      - in: query
        name: group_id
        description: The id of a group whos pool to search
      - in: query
        name: has_geo
        description: Any photo that has been geotagged, or if the value is 0 any photo
          that has not been geotagged
      - in: query
        name: hbox
        description: A comma-delimited list of 4 values defining the Bounding Box
          of the area that will be searched
      - in: query
        name: is_commons
        description: Limit the scope of the search to only photos that are part of
          the Flickr Commons project
      - in: query
        name: is_gallery
        description: Limit the scope of the search to only photos that are in a gallery?
          Default is false, search all photos
      - in: query
        name: is_getty
        description: Limit the scope of the search to only photos that are for sale
          on Getty
      - in: query
        name: lat
        description: A valid latitude, in decimal format, for doing radial geo queries
      - in: query
        name: license
        description: The license id for photos (for possible values see the flickr
      - in: query
        name: lon
        description: A valid longitude, in decimal format, for doing radial geo queries
      - in: query
        name: machine_tags
        description: Machine tag(s)
      - in: query
        name: machine_tag_mode
        description: Either any for an OR combination of tags, or all for an AND combination
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
        name: place_id
        description: A Flickr place id
      - in: query
        name: privacy_filter
        description: Return photos only matching a certain privacy level
      - in: query
        name: radius
        description: A valid radius used for geo queries, greater than zero and less
          than 20 miles (or 32 kilometers), for use with point-based geo queries
      - in: query
        name: radius_units
        description: The unit of measure when doing radial geo queries
      - in: query
        name: safe_search
        description: Safe search setting
      - in: query
        name: sort
        description: The order in which to sort returned photos
      - in: query
        name: tags
        description: A comma-delimited list of tags
      - in: query
        name: tag_mode
        description: Either any for an OR combination of tags, or all for an AND combination
      - in: query
        name: text
        description: A free text search
      - in: query
        name: user_id
        description: The NSID of the user whos photo to search
      - in: query
        name: woe_id
        description: A 32-bit identifier that uniquely represents spatial entities
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Search
  /rest/?method=flickr.photos.setContentType:
    post:
      summary: Photos Set Content Type
      description: Set the content type of a photo.
      operationId: postRestMethodFlickr.photos.setcontenttype
      x-api-path-slug: restmethodflickr-photos-setcontenttype-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: content_type
        description: The content type of the photo
      - in: query
        name: photo_id
        description: The id of the photo to set the adultness of
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetContentType
  /rest/?method=flickr.photos.setDates:
    post:
      summary: Photos Set Dates
      description: Set one or both of the dates for a photo.
      operationId: postRestMethodFlickr.photos.setdates
      x-api-path-slug: restmethodflickr-photos-setdates-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date_posted
        description: The date the photo was uploaded to flickr (see the dates documentation)
      - in: query
        name: date_taken
        description: The date the photo was taken (see the dates documentation)
      - in: query
        name: date_taken_granularity
        description: The granularity of the date the photo was taken (see the dates
          documentation)
      - in: query
        name: photo_id
        description: The id of the photo to edit dates for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetDates
  /rest/?method=flickr.photos.setMeta:
    post:
      summary: Photos Set Meta
      description: Set the meta information for a photo.
      operationId: postRestMethodFlickr.photos.setmeta
      x-api-path-slug: restmethodflickr-photos-setmeta-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: description
        description: The description for the photo
      - in: query
        name: photo_id
        description: The id of the photo to set information for
      - in: query
        name: title
        description: The title for the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetMeta
  /rest/?method=flickr.photos.setPerms:
    post:
      summary: Photos Set Perms
      description: Set permissions for a photo.
      operationId: postRestMethodFlickr.photos.setperms
      x-api-path-slug: restmethodflickr-photos-setperms-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: is_family
        description: 1 to make the photo visible to family when private, 0 to not
      - in: query
        name: is_friend
        description: 1 to make the photo visible to friends when private, 0 to not
      - in: query
        name: is_public
        description: 1 to set the photo to public, 0 to set it to private
      - in: query
        name: perm_addmeta
        description: Who can add notes and tags to the photo
      - in: query
        name: perm_comment
        description: Who can add comments to the photo and its notes
      - in: query
        name: photo_id
        description: The id of the photo to set permissions for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetPerms
  /rest/?method=flickr.photos.setSafetyLevel:
    post:
      summary: Photos Set Safety Level
      description: Set the safety level of a photo.
      operationId: postRestMethodFlickr.photos.setsafetylevel
      x-api-path-slug: restmethodflickr-photos-setsafetylevel-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: hidden
        description: Whether or not to additionally hide the photo from public searches
      - in: query
        name: photo_id
        description: The id of the photo to set the adultness of
      - in: query
        name: safety_level
        description: The safety level of the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetSafetyLevel
  /rest/?method=flickr.photos.setTags:
    post:
      summary: Photos Set Tags
      description: Set the tags for a photo.
      operationId: postRestMethodFlickr.photos.settags
      x-api-path-slug: restmethodflickr-photos-settags-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to set the tags for
      - in: query
        name: tags
        description: All tags for the photo (as a single space-delimited string)
      responses:
        200:
          description: OK
      tags:
      - Photos
      - SetTags
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