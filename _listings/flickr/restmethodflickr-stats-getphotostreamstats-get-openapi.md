---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Stats Get Photostream Stats
  description: Get the number of views on a user's photostream for a given date.
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
  /rest/?method=flickr.people.getPublicPhotos:
    get:
      summary: People Get Public Photos
      description: Get a list of public photos for the given user.
      operationId: getRestMethodFlickr.people.getpublicphotos
      x-api-path-slug: restmethodflickr-people-getpublicphotos-get
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
      - GetPublicPhotos
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
  /rest/?method=flickr.photos.comments.addComment:
    post:
      summary: Photos Comments Add Comment
      description: Add comment to a photo as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.addcomment
      x-api-path-slug: restmethodflickr-photos-comments-addcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_text
        description: Text of the comment
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to add a comment to
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - AddComment
  /rest/?method=flickr.photos.comments.deleteComment:
    post:
      summary: Photos Comments Delete Comment
      description: Delete comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.deletecomment
      x-api-path-slug: restmethodflickr-photos-comments-deletecomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to delete a comment from
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - DeleteComment
  /rest/?method=flickr.photos.comments.editComment:
    post:
      summary: Photos Comments Edit Comment
      description: Edit the text of a comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photos.comments.editcomment
      x-api-path-slug: restmethodflickr-photos-comments-editcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to edit
      - in: query
        name: comment_text
        description: Update the comment to this text
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - EditComment
  /rest/?method=flickr.photos.comments.getList:
    get:
      summary: Photos Comments Get List
      description: Returns the comments for a photo.
      operationId: getRestMethodFlickr.photos.comments.getlist
      x-api-path-slug: restmethodflickr-photos-comments-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_comment_date
        description: Maximum date that a comment was added
      - in: query
        name: min_comment_date
        description: Minimum date that a comment was added
      - in: query
        name: photo_id
        description: The id of the photo to fetch comments for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Comments
      - GetList
  /rest/?method=flickr.photos.comments.getRecentForContacts:
    get:
      summary: Photos Comments Get Recent For Contacts
      description: Return the list of photos belonging to your contacts that have
        been commented on recently.
      operationId: getRestMethodFlickr.photos.comments.getrecentforcontacts
      x-api-path-slug: restmethodflickr-photos-comments-getrecentforcontacts-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: contacts_filter
        description: A comma-separated list of contact NSIDs to limit the scope of
          the query to
      - in: query
        name: date_lastcomment
        description: Limits the resultset to photos that have been commented on since
          this date
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
      - Comments
      - GetRecentForContacts
  /rest/?method=flickr.photos.geo.batchCorrectLocation:
    post:
      summary: Photos Geo Batch Correct Location
      description: Correct the places hierarchy for all the photos for a user at a
        given latitude, longitude and accuracy. Batch corrections are processed in
        a delayed queue so it may take a few minutes before the changes are reflected
        in a user's photos.
      operationId: postRestMethodFlickr.photos.geo.batchcorrectlocation
      x-api-path-slug: restmethodflickr-photos-geo-batchcorrectlocation-post
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the photos to be updated
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: lat
        description: The latitude of the photos to be updated whose valid range is
          -90 to 90
      - in: query
        name: lon
        description: The longitude of the photos to be updated whose valid range is
          -180 to 180
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where on Earch (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - BatchCorrectLocation
  /rest/?method=flickr.photos.geo.correctLocation:
    post:
      summary: Photos Geo Correct Location
      description: Corrects a photo's location.
      operationId: postRestMethodFlickr.photos.geo.correctlocation
      x-api-path-slug: restmethodflickr-photos-geo-correctlocation-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The ID of the photo whose WOE location is being corrected
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where on Earch (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - CorrectLocation
  /rest/?method=flickr.photos.geo.getLocation:
    get:
      summary: Photos Geo Get Location
      description: Get the geo data (latitude and longitude and the accuracy level)
        for a photo.
      operationId: getRestMethodFlickr.photos.geo.getlocation
      x-api-path-slug: restmethodflickr-photos-geo-getlocation-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo you want to retrieve location data for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - GetLocation
  /rest/?method=flickr.photos.geo.getPerms:
    get:
      summary: Photos Geo Get Perms
      description: Get permissions for who may view geo data for a photo.
      operationId: getRestMethodFlickr.photos.geo.getperms
      x-api-path-slug: restmethodflickr-photos-geo-getperms-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo you want to get permissions for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - GetPerms
  /rest/?method=flickr.photos.geo.photosForLocation:
    get:
      summary: Photos Geo Photos For Location
      description: Return a list of photos for the calling user at a specific latitude,
        longitude and accuracy
      operationId: getRestMethodFlickr.photos.geo.photosforlocation
      x-api-path-slug: restmethodflickr-photos-geo-photosforlocation-get
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
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
        name: lat
        description: The latitude whose valid range is -90 to 90
      - in: query
        name: lon
        description: The longitude whose valid range is -180 to 180
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
      - Geo
      - PhotosForLocation
  /rest/?method=flickr.photos.geo.removeLocation:
    post:
      summary: Photos Geo Remove Location
      description: Removes the geo data associated with a photo.
      operationId: postRestMethodFlickr.photos.geo.removelocation
      x-api-path-slug: restmethodflickr-photos-geo-removelocation-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The ID of the photo you want to remove location data from
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - RemoveLocation
  /rest/?method=flickr.photos.geo.setContext:
    post:
      summary: Photos Geo Set Context
      description: 'Indicate the state of a photo''s geotagginess beyond latitude
        and longitude. Note : photos passed to this method must already be geotagged
        (using the flickr.photos.geo.setLocation method).'
      operationId: postRestMethodFlickr.photos.geo.setcontext
      x-api-path-slug: restmethodflickr-photos-geo-setcontext-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: context
        description: Context is a numeric value representing the photos geotagginess
          beyond latitude and longitude
      - in: query
        name: photo_id
        description: The ID of the photo you want to set context data for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - SetContext
  /rest/?method=flickr.photos.geo.setLocation:
    post:
      summary: Photos Geo Set Location
      description: Sets the geo data (latitude and longitude and, optionally, the
        accuracy level) for a photo. Before users may assign location data to a photo
        they must define who, by default, may view that information. Users can edit
        this preference at http://www.flickr.com/account/geo/privacy/. If a user has
        not set this preference, the API method will return an error.
      operationId: postRestMethodFlickr.photos.geo.setlocation
      x-api-path-slug: restmethodflickr-photos-geo-setlocation-post
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: context
        description: Context is a numeric value representing the photos geotagginess
          beyond latitude and longitude
      - in: query
        name: format
        description: Response format
      - in: query
        name: lat
        description: The latitude whose valid range is -90 to 90
      - in: query
        name: lon
        description: The longitude whose valid range is -180 to 180
      - in: query
        name: photo_id
        description: The id of the photo you want to retrieve location data for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - SetLocation
  /rest/?method=flickr.photos.geo.setPerms:
    get:
      summary: Photos Geo Set Perms
      description: Set the permission for who may view the geo data associated with
        a photo.
      operationId: getRestMethodFlickr.photos.geo.setperms
      x-api-path-slug: restmethodflickr-photos-geo-setperms-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: is_contact
        description: 1 to set viewing permissions for the photos location data to
          contacts, 0 to set it to private
      - in: query
        name: is_family
        description: 1 to set viewing permissions for the photos location data to
          family, 0 to set it to private
      - in: query
        name: is_friend
        description: 1 to set viewing permissions for the photos location data to
          friends, 0 to set it to private
      - in: query
        name: is_public
        description: 1 to set viewing permissions for the photos location data to
          public, 0 to set it to private
      - in: query
        name: photo_id
        description: The id of the photo to get permissions for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Geo
      - SetPerms
  /rest/?method=flickr.photos.licenses.getInfo:
    get:
      summary: Photos Licenses Get Info
      description: Fetches a list of available photo licenses for Flickr.
      operationId: getRestMethodFlickr.photos.licenses.getinfo
      x-api-path-slug: restmethodflickr-photos-licenses-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Licenses
      - GetInfo
  /rest/?method=flickr.photos.licenses.setInfo:
    post:
      summary: Photos Licenses Set Info
      description: Sets the license for a photo.
      operationId: postRestMethodFlickr.photos.licenses.setinfo
      x-api-path-slug: restmethodflickr-photos-licenses-setinfo-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: license_id
        description: The license to apply, or 0 (zero) to remove the current license
      - in: query
        name: photo_id
        description: The id of the photo you want to update the license for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Licenses
      - SetInfo
  /rest/?method=flickr.photos.notes.add:
    post:
      summary: Photos Notes Add
      description: Add a note to a photo. Coordinates and sizes are in pixels, based
        on the 500px image size shown on individual photo pages.
      operationId: postRestMethodFlickr.photos.notes.add
      x-api-path-slug: restmethodflickr-photos-notes-add-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: note_h
        description: The height of the note
      - in: query
        name: note_text
        description: The description of the note
      - in: query
        name: note_w
        description: The width of the note
      - in: query
        name: note_x
        description: The left coordinate of the note
      - in: query
        name: note_y
        description: The top coordinate of the note
      - in: query
        name: photo_id
        description: The id of the photo to add a note to
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Notes
      - Add
  /rest/?method=flickr.photos.notes.delete:
    post:
      summary: Photos Notes Delete
      description: Delete a note from a photo.
      operationId: postRestMethodFlickr.photos.notes.delete
      x-api-path-slug: restmethodflickr-photos-notes-delete-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: note_id
        description: The id of the note to delete
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Notes
      - Delete
  /rest/?method=flickr.photos.notes.edit:
    post:
      summary: Photos Notes Edit
      description: Edit a note on a photo. Coordinates and sizes are in pixels, based
        on the 500px image size shown on individual photo pages.
      operationId: postRestMethodFlickr.photos.notes.edit
      x-api-path-slug: restmethodflickr-photos-notes-edit-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: note_h
        description: The height of the note
      - in: query
        name: note_id
        description: The id of the note to edit
      - in: query
        name: note_text
        description: The description of the note
      - in: query
        name: note_w
        description: The width of the note
      - in: query
        name: note_x
        description: The left coordinate of the note
      - in: query
        name: note_y
        description: The top coordinate of the note
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Notes
      - Edit
  /rest/?method=flickr.photos.people.add:
    post:
      summary: Photos People Add
      description: Add a person to a photo. Coordinates and sizes are in pixels, based
        on the 500px image size shown on individual photo pages.
      operationId: postRestMethodFlickr.photos.people.add
      x-api-path-slug: restmethodflickr-photos-people-add-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: person_h
        description: The height (in pixels) of the box around the person
      - in: query
        name: person_w
        description: The width (in pixels) of the box around the person
      - in: query
        name: person_x
        description: The left-most pixel co-ordinate of the box around the person
      - in: query
        name: person_y
        description: The top-most pixel co-ordinate of the box around the person
      - in: query
        name: photo_id
        description: The id of the photo to add a person to
      - in: query
        name: user_id
        description: The NSID of the user to add to the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
      - Add
  /rest/?method=flickr.photos.people.delete:
    post:
      summary: Photos People Delete
      description: Remove a person from a photo.
      operationId: postRestMethodFlickr.photos.people.delete
      x-api-path-slug: restmethodflickr-photos-people-delete-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to remove a person from
      - in: query
        name: user_id
        description: The NSID of the user to remove from the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
      - Delete
  /rest/?method=flickr.photos.people.deleteCoords:
    post:
      summary: Photos People Delete Coords
      description: Remove the bounding box from a person in a photo
      operationId: postRestMethodFlickr.photos.people.deletecoords
      x-api-path-slug: restmethodflickr-photos-people-deletecoords-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photo_id
        description: The id of the photo to edit a person in
      - in: query
        name: user_id
        description: The NSID of the user whose bounding box you want to remove
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
      - DeleteCoords
  /rest/?method=flickr.photos.people.editCoords:
    post:
      summary: Photos People Edit Coords
      description: Edit the bounding box of an existing person on a photo.
      operationId: postRestMethodFlickr.photos.people.editcoords
      x-api-path-slug: restmethodflickr-photos-people-editcoords-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: person_h
        description: The height (in pixels) of the box around the person
      - in: query
        name: person_w
        description: The width (in pixels) of the box around the person
      - in: query
        name: person_x
        description: The left-most pixel co-ordinate of the box around the person
      - in: query
        name: person_y
        description: The top-most pixel co-ordinate of the box around the person
      - in: query
        name: photo_id
        description: The id of the photo to edit a person in
      - in: query
        name: user_id
        description: The NSID of the user to edit in the photo
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
      - EditCoords
  /rest/?method=flickr.photos.people.getList:
    get:
      summary: Photos People Get List
      description: Get a list of people in a given photo.
      operationId: getRestMethodFlickr.photos.people.getlist
      x-api-path-slug: restmethodflickr-photos-people-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to get a list of people for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - People
      - GetList
  /rest/?method=flickr.photos.transform.rotate:
    post:
      summary: Photos Transform Rotate
      description: Rotate a photo.
      operationId: postRestMethodFlickr.photos.transform.rotate
      x-api-path-slug: restmethodflickr-photos-transform-rotate-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: degrees
        description: The amount of degrees by which to rotate the photo (clockwise)
          from its current orientation
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to rotate
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Transform
      - Rotate
  /rest/?method=flickr.photos.upload.checkTickets:
    get:
      summary: Photos Upload Check Tickets
      description: Checks the status of one or more asynchronous photo upload tickets.
      operationId: getRestMethodFlickr.photos.upload.checktickets
      x-api-path-slug: restmethodflickr-photos-upload-checktickets-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: tickets
        description: A comma-delimited list of ticket ids
      responses:
        200:
          description: OK
      tags:
      - Photos
      - Upload
      - CheckTickets
  /rest/?method=flickr.photosets.addPhoto:
    post:
      summary: Photosets Add Photo
      description: Add a photo to the end of an existing photoset.
      operationId: postRestMethodFlickr.photosets.addphoto
      x-api-path-slug: restmethodflickr-photosets-addphoto-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to add a photo to
      - in: query
        name: photo_id
        description: The id of the photo to add to the set
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - AddPhoto
  /rest/?method=flickr.photosets.create:
    post:
      summary: Photosets Create
      description: Create a new photoset for the calling user.
      operationId: postRestMethodFlickr.photosets.create
      x-api-path-slug: restmethodflickr-photosets-create-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: description
        description: A description of the photoset
      - in: query
        name: format
        description: Response format
      - in: query
        name: primary_photo_id
        description: The id of the photo to represent this set
      - in: query
        name: title
        description: A title for the photoset
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Create
  /rest/?method=flickr.photosets.delete:
    post:
      summary: Photosets Delete
      description: Delete a new photoset.
      operationId: postRestMethodFlickr.photosets.delete
      x-api-path-slug: restmethodflickr-photosets-delete-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to delete
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Delete
  /rest/?method=flickr.photosets.editMeta:
    post:
      summary: Photosets Edit Meta
      description: Modify the meta-data for a photoset.
      operationId: postRestMethodFlickr.photosets.editmeta
      x-api-path-slug: restmethodflickr-photosets-editmeta-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: description
        description: A description of the photoset
      - in: query
        name: photoset_id
        description: The id of the photoset to modify
      - in: query
        name: title
        description: The new title for the photoset
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - EditMeta
  /rest/?method=flickr.photosets.editPhotos:
    post:
      summary: Photosets Edit Photos
      description: Modify the photos in a photoset. Use this method to add, remove
        and re-order photos.
      operationId: postRestMethodFlickr.photosets.editphotos
      x-api-path-slug: restmethodflickr-photosets-editphotos-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to modify
      - in: query
        name: photo_ids
        description: A comma-delimited list of photo ids to include in the set
      - in: query
        name: primary_photo_id
        description: The id of the photo to use as the primary photo for the set
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - EditPhotos
  /rest/?method=flickr.photosets.getContext:
    get:
      summary: Photosets Get Context
      description: Returns next and previous photos for a photo in a set.
      operationId: getRestMethodFlickr.photosets.getcontext
      x-api-path-slug: restmethodflickr-photosets-getcontext-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset for which to fetch the photos context
      - in: query
        name: photo_id
        description: The id of the photo to fetch the context for
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - GetContext
  /rest/?method=flickr.photosets.getInfo:
    get:
      summary: Photosets Get Info
      description: Gets information about a photoset.
      operationId: getRestMethodFlickr.photosets.getinfo
      x-api-path-slug: restmethodflickr-photosets-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The ID of the photoset to fetch information for
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - GetInfo
  /rest/?method=flickr.photosets.getList:
    get:
      summary: Photosets Get List
      description: Returns the photosets belonging to the specified user.
      operationId: getRestMethodFlickr.photosets.getlist
      x-api-path-slug: restmethodflickr-photosets-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The NSID of the user to get a photoset list for
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - GetList
  /rest/?method=flickr.photosets.getPhotos:
    get:
      summary: Photosets Get Photos
      description: Get the list of photos in a set.
      operationId: getRestMethodFlickr.photosets.getphotos
      x-api-path-slug: restmethodflickr-photosets-getphotos-get
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
        name: media
        description: Filter results by media type
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: photoset_id
        description: The id of the photoset to return the photos for
      - in: query
        name: privacy_filter
        description: Return photos only matching a certain privacy level
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - GetPhotos
  /rest/?method=flickr.photosets.orderSets:
    post:
      summary: Photosets Order Sets
      description: Set the order of photosets for the calling user.
      operationId: postRestMethodFlickr.photosets.ordersets
      x-api-path-slug: restmethodflickr-photosets-ordersets-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_ids
        description: A comma delimited list of photoset IDs, ordered with the set
          to show first, first in the list
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - OrderSets
  /rest/?method=flickr.photosets.removePhoto:
    post:
      summary: Photosets Remove Photo
      description: Remove a photo from a photoset.
      operationId: postRestMethodFlickr.photosets.removephoto
      x-api-path-slug: restmethodflickr-photosets-removephoto-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to remove a photo from
      - in: query
        name: photo_id
        description: The id of the photo to remove to the set
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - RemovePhoto
  /rest/?method=flickr.photosets.removePhotos:
    post:
      summary: Photosets Remove Photos
      description: Remove multiple photos from a photoset.
      operationId: postRestMethodFlickr.photosets.removephotos
      x-api-path-slug: restmethodflickr-photosets-removephotos-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to remove photos from
      - in: query
        name: photo_ids
        description: Comma-delimited list of photo ids to remove from the photoset
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - RemovePhotos
  /rest/?method=flickr.photosets.reorderPhotos:
    post:
      summary: Photosets Reorder Photos
      description: Update the order of photos in a photoset.
      operationId: postRestMethodFlickr.photosets.reorderphotos
      x-api-path-slug: restmethodflickr-photosets-reorderphotos-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to reorder
      - in: query
        name: photo_ids
        description: Ordered, comma-delimited list of photo ids
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - ReorderPhotos
  /rest/?method=flickr.photosets.setPrimaryPhoto:
    post:
      summary: Photosets Set Primary Photo
      description: Set photoset primary photo
      operationId: postRestMethodFlickr.photosets.setprimaryphoto
      x-api-path-slug: restmethodflickr-photosets-setprimaryphoto-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_id
        description: The id of the photoset to set primary photo of
      - in: query
        name: photo_id
        description: The id of the photo to set as primary
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - SetPrimaryPhoto
  /rest/?method=flickr.photosets.comments.addComment:
    post:
      summary: Photosets Comments Add Comment
      description: Add a comment to a photoset.
      operationId: postRestMethodFlickr.photosets.comments.addcomment
      x-api-path-slug: restmethodflickr-photosets-comments-addcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_text
        description: Text of the comment
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset to add a comment to
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - AddComment
  /rest/?method=flickr.photosets.comments.deleteComment:
    post:
      summary: Photosets Comments Delete Comment
      description: Delete a photoset comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photosets.comments.deletecomment
      x-api-path-slug: restmethodflickr-photosets-comments-deletecomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to delete from a photoset
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - DeleteComment
  /rest/?method=flickr.photosets.comments.editComment:
    post:
      summary: Photosets Comments Edit Comment
      description: Edit the text of a comment as the currently authenticated user.
      operationId: postRestMethodFlickr.photosets.comments.editcomment
      x-api-path-slug: restmethodflickr-photosets-comments-editcomment-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: comment_id
        description: The id of the comment to edit
      - in: query
        name: comment_text
        description: Update the comment to this text
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - EditComment
  /rest/?method=flickr.photosets.comments.getList:
    get:
      summary: Photosets Comments Get List
      description: Returns the comments for a photoset.
      operationId: getRestMethodFlickr.photosets.comments.getlist
      x-api-path-slug: restmethodflickr-photosets-comments-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset to fetch comments for
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - Comments
      - GetList
  /rest/?method=flickr.places.getChildrenWithPhotosPublic:
    get:
      summary: Places Get Children With Photos Public
      description: Return a list of locations with public photos that are parented
        by a Where on Earth (WOE) or Places ID.
      operationId: getRestMethodFlickr.places.getchildrenwithphotospublic
      x-api-path-slug: restmethodflickr-places-getchildrenwithphotospublic-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetChildrenWithPhotosPublic
  /rest/?method=flickr.stats.getPhotoStats:
    get:
      summary: Stats Get Photo Stats
      description: Get the number of views, comments and favorites on a photo for
        a given date.
      operationId: getRestMethodFlickr.stats.getphotostats
      x-api-path-slug: restmethodflickr-stats-getphotostats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: photo_id
        description: The id of the photo to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotoStats
  /rest/?method=flickr.stats.getPhotosetDomains:
    get:
      summary: Stats Get Photoset Domains
      description: Get a list of referring domains for a photoset.
      operationId: getRestMethodFlickr.stats.getphotosetdomains
      x-api-path-slug: restmethodflickr-stats-getphotosetdomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetDomains
  /rest/?method=flickr.stats.getPhotosetReferrers:
    get:
      summary: Stats Get Photoset Referrers
      description: Get a list of referring domains for a photoset.
      operationId: getRestMethodFlickr.stats.getphotosetreferrers
      x-api-path-slug: restmethodflickr-stats-getphotosetreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetReferrers
  /rest/?method=flickr.stats.getPhotosetStats:
    get:
      summary: Stats Get Photoset Stats
      description: Get the number of views on a photoset for a given date.
      operationId: getRestMethodFlickr.stats.getphotosetstats
      x-api-path-slug: restmethodflickr-stats-getphotosetstats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: photoset_id
        description: The id of the photoset to get stats for
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotosetStats
  /rest/?method=flickr.stats.getPhotostreamDomains:
    get:
      summary: Stats Get Photostream Domains
      description: Get a list of referring domains for a photostream.
      operationId: getRestMethodFlickr.stats.getphotostreamdomains
      x-api-path-slug: restmethodflickr-stats-getphotostreamdomains-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamDomains
  /rest/?method=flickr.stats.getPhotostreamReferrers:
    get:
      summary: Stats Get Photostream Referrers
      description: Get a list of referrers from a given domain to a user's photostream
      operationId: getRestMethodFlickr.stats.getphotostreamreferrers
      x-api-path-slug: restmethodflickr-stats-getphotostreamreferrers-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: domain
        description: The domain to return referrers for
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of domains to return per page
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamReferrers
  /rest/?method=flickr.stats.getPhotostreamStats:
    get:
      summary: Stats Get Photostream Stats
      description: Get the number of views on a user's photostream for a given date.
      operationId: getRestMethodFlickr.stats.getphotostreamstats
      x-api-path-slug: restmethodflickr-stats-getphotostreamstats-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: date
        description: Stats will be returned for this date
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Stats
      - GetPhotostreamStats
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