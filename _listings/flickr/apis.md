---
name: Flickr
x-slug: flickr
description: Flickr (pronounced flicker) is an image hosting and video hosting website,
  and web services suite that was created by Ludicorp in 2004 and acquired by Yahoo
  in 2005. In addition to being a popular website for users to share and embed personal
  photographs, and effectively an online community, the service is widely used by
  photo researchers and by bloggers to host images that they embed in blogs and social
  media.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Photos
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/apis.md
specificationVersion: "0.14"
apis:
- name: Flickr Activity User Photos
  x-api-slug: flickr
  description: Returns a list of recent activity on photos commented on by the calling
    user. Do not poll this method more than once an hour.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.activity.userPhotos
  tags: Activity,UserPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-activity-userphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-activity-userphotos-get-openapi.md
- name: Flickr Galleries Edit Photos
  x-api-slug: flickr
  description: Modify the photos in a gallery. Use this method to add, remove and
    re-order photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.editPhotos
  tags: Galleries,EditPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-galleries-editphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-galleries-editphotos-post-openapi.md
- name: Flickr Galleries Get Photos
  x-api-slug: flickr
  description: Return the list of photos for a gallery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.galleries.getPhotos
  tags: Galleries,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-galleries-getphotos-get-openapi.md
- name: Flickr Groups Pools Get Photos
  x-api-slug: flickr
  description: Returns a list of pool photos for a given group, based on the permissions
    of the group and the user logged in (if any).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.groups.pools.getPhotos
  tags: Groups,Pools,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-groups-pools-getphotos-get-openapi.md
- name: Flickr Panda Get Photos
  x-api-slug: flickr
  description: Ask the Flickr Pandas for a list of recent public (and "safe") photos.
    More information about the pandas can be found on the dev blog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.panda.getPhotos
  tags: Panda,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-panda-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-panda-getphotos-get-openapi.md
- name: Flickr People Get Photos
  x-api-slug: flickr
  description: Return photos from the given user's photostream. Only photos visible
    to the calling user will be returned. This method must be authenticated; to return
    public photos for a user, use flickr.people.getPublicPhotos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPhotos
  tags: People,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getphotos-get-openapi.md
- name: Flickr People Get Photos Of
  x-api-slug: flickr
  description: Returns a list of photos containing a particular Flickr member.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPhotosOf
  tags: People,GetPhotosOf
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getphotosof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getphotosof-get-openapi.md
- name: Flickr People Get Public Photos
  x-api-slug: flickr
  description: Get a list of public photos for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPublicPhotos
  tags: People,GetPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-openapi.md
- name: Flickr Photos Add Tags
  x-api-slug: flickr
  description: Add tags to a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.addTags
  tags: Photos,AddTags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-addtags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-addtags-post-openapi.md
- name: Flickr Photos Delete
  x-api-slug: flickr
  description: Delete a photo from Flickr.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.delete
  tags: Photos,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-delete-post-openapi.md
- name: Flickr Photos Get All Contexts
  x-api-slug: flickr
  description: Returns all visible sets and pools the photo belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getAllContexts
  tags: Photos,GetAllContexts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getallcontexts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getallcontexts-get-openapi.md
- name: Flickr Photos Get Contacts Photos
  x-api-slug: flickr
  description: Fetch a list of recent photos from the calling users' contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContactsPhotos
  tags: Photos,GetContactsPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontactsphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontactsphotos-get-openapi.md
- name: Flickr Photos Get Contacts Public Photos
  x-api-slug: flickr
  description: Fetch a list of recent public photos from a users' contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContactsPublicPhotos
  tags: Photos,GetContactsPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-openapi.md
- name: Flickr Photos Get Context
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContext
  tags: Photos,GetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcontext-get-openapi.md
- name: Flickr Photos Get Counts
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getCounts
  tags: Photos,GetCounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getcounts-get-openapi.md
- name: Flickr Photos Get Exif
  x-api-slug: flickr
  description: Retrieves a list of EXIF/TIFF/GPS tags for a given photo. The calling
    user must have permission to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getExif
  tags: Photos,GetExif
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getexif-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getexif-get-openapi.md
- name: Flickr Photos Get Favorites
  x-api-slug: flickr
  description: Returns the list of people who have favorited a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getFavorites
  tags: Photos,GetFavorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getfavorites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getfavorites-get-openapi.md
- name: Flickr Photos Get Info
  x-api-slug: flickr
  description: Get information about a photo. The calling user must have permission
    to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getInfo
  tags: Photos,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getinfo-get-openapi.md
- name: Flickr Photos Get Not In Set
  x-api-slug: flickr
  description: Returns a list of your photos that are not part of any sets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getNotInSet
  tags: Photos,GetNotInSet
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getnotinset-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getnotinset-get-openapi.md
- name: Flickr Photos Get Perms
  x-api-slug: flickr
  description: Get permissions for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getPerms
  tags: Photos,GetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getperms-get-openapi.md
- name: Flickr Photos Get Recent
  x-api-slug: flickr
  description: Returns the list of people who have favorited a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getRecent
  tags: Photos,GetRecent
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getrecent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getrecent-get-openapi.md
- name: Flickr Photos Get Sizes
  x-api-slug: flickr
  description: Returns the available sizes for a photo. The calling user must have
    permission to view the photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getSizes
  tags: Photos,GetSizes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getsizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getsizes-get-openapi.md
- name: Flickr Photos Get Untagged
  x-api-slug: flickr
  description: Returns a list of your photos that are not tagged.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getUntagged
  tags: Photos,GetUntagged
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getuntagged-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getuntagged-get-openapi.md
- name: Flickr Photos Get With Geo Data
  x-api-slug: flickr
  description: Returns a list of your geo-tagged photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getWithGeoData
  tags: Photos,GetWithGeoData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getwithgeodata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getwithgeodata-get-openapi.md
- name: Flickr Photos Get Without Geo Data
  x-api-slug: flickr
  description: Returns a list of your photos which haven't been geo-tagged.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getWithoutGeoData
  tags: Photos,GetWithoutGeoData
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getwithoutgeodata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getwithoutgeodata-get-openapi.md
- name: Flickr Photos Get Recently Updated
  x-api-slug: flickr
  description: Return a list of your photos that have been recently created or which
    have been recently modified. Recently modified may mean that the photo's metadata
    (title, description, tags) may have been changed or a comment has been added (or
    just modified somehow :-)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getRecentlyUpdated
  tags: Photos,GetRecentlyd
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getrecentlyupdated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-getrecentlyupdated-get-openapi.md
- name: Flickr Photos Remove Tag
  x-api-slug: flickr
  description: Remove a tag from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.removeTag
  tags: Photos,RemoveTag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-removetag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-removetag-post-openapi.md
- name: Flickr Photos Search
  x-api-slug: flickr
  description: Return a list of photos matching some criteria. Only photos visible
    to the calling user will be returned. To return private or semi-private photos,
    the caller must be authenticated with 'read' permissions, and have permission
    to view the photos. Unauthenticated calls will only return public photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.search
  tags: Photos,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-search-get-openapi.md
- name: Flickr Photos Set Content Type
  x-api-slug: flickr
  description: Set the content type of a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setContentType
  tags: Photos,SetContentType
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setcontenttype-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setcontenttype-post-openapi.md
- name: Flickr Photos Set Dates
  x-api-slug: flickr
  description: Set one or both of the dates for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setDates
  tags: Photos,SetDates
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setdates-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setdates-post-openapi.md
- name: Flickr Photos Set Meta
  x-api-slug: flickr
  description: Set the meta information for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setMeta
  tags: Photos,SetMeta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setmeta-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setmeta-post-openapi.md
- name: Flickr Photos Set Perms
  x-api-slug: flickr
  description: Set permissions for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setPerms
  tags: Photos,SetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setperms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setperms-post-openapi.md
- name: Flickr Photos Set Safety Level
  x-api-slug: flickr
  description: Set the safety level of a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setSafetyLevel
  tags: Photos,SetSafetyLevel
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setsafetylevel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-setsafetylevel-post-openapi.md
- name: Flickr Photos Set Tags
  x-api-slug: flickr
  description: Set the tags for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.setTags
  tags: Photos,SetTags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-settags-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-settags-post-openapi.md
- name: Flickr Photos Comments Add Comment
  x-api-slug: flickr
  description: Add comment to a photo as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.addComment
  tags: Photos,Comments,AddComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-addcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-addcomment-post-openapi.md
- name: Flickr Photos Comments Delete Comment
  x-api-slug: flickr
  description: Delete comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.deleteComment
  tags: Photos,Comments,DeleteComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-deletecomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-deletecomment-post-openapi.md
- name: Flickr Photos Comments Edit Comment
  x-api-slug: flickr
  description: Edit the text of a comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.editComment
  tags: Photos,Comments,EditComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-editcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-editcomment-post-openapi.md
- name: Flickr Photos Comments Get List
  x-api-slug: flickr
  description: Returns the comments for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.getList
  tags: Photos,Comments,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-getlist-get-openapi.md
- name: Flickr Photos Comments Get Recent For Contacts
  x-api-slug: flickr
  description: Return the list of photos belonging to your contacts that have been
    commented on recently.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.comments.getRecentForContacts
  tags: Photos,Comments,GetRecentForContacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-getrecentforcontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-comments-getrecentforcontacts-get-openapi.md
- name: Flickr Photos Geo Batch Correct Location
  x-api-slug: flickr
  description: Correct the places hierarchy for all the photos for a user at a given
    latitude, longitude and accuracy. Batch corrections are processed in a delayed
    queue so it may take a few minutes before the changes are reflected in a user's
    photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.batchCorrectLocation
  tags: Photos,Geo,BatchCorrectLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-batchcorrectlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-batchcorrectlocation-post-openapi.md
- name: Flickr Photos Geo Correct Location
  x-api-slug: flickr
  description: Corrects a photo's location.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.correctLocation
  tags: Photos,Geo,CorrectLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-correctlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-correctlocation-post-openapi.md
- name: Flickr Photos Geo Get Location
  x-api-slug: flickr
  description: Get the geo data (latitude and longitude and the accuracy level) for
    a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.getLocation
  tags: Photos,Geo,GetLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-getlocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-getlocation-get-openapi.md
- name: Flickr Photos Geo Get Perms
  x-api-slug: flickr
  description: Get permissions for who may view geo data for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.getPerms
  tags: Photos,Geo,GetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-getperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-getperms-get-openapi.md
- name: Flickr Photos Geo Photos For Location
  x-api-slug: flickr
  description: Return a list of photos for the calling user at a specific latitude,
    longitude and accuracy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.photosForLocation
  tags: Photos,Geo,PhotosForLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-photosforlocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-photosforlocation-get-openapi.md
- name: Flickr Photos Geo Remove Location
  x-api-slug: flickr
  description: Removes the geo data associated with a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.removeLocation
  tags: Photos,Geo,RemoveLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-removelocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-removelocation-post-openapi.md
- name: Flickr Photos Geo Set Context
  x-api-slug: flickr
  description: 'Indicate the state of a photo''s geotagginess beyond latitude and
    longitude. Note : photos passed to this method must already be geotagged (using
    the flickr.photos.geo.setLocation method).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setContext
  tags: Photos,Geo,SetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setcontext-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setcontext-post-openapi.md
- name: Flickr Photos Geo Set Location
  x-api-slug: flickr
  description: Sets the geo data (latitude and longitude and, optionally, the accuracy
    level) for a photo. Before users may assign location data to a photo they must
    define who, by default, may view that information. Users can edit this preference
    at http://www.flickr.com/account/geo/privacy/. If a user has not set this preference,
    the API method will return an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setLocation
  tags: Photos,Geo,SetLocation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setlocation-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setlocation-post-openapi.md
- name: Flickr Photos Geo Set Perms
  x-api-slug: flickr
  description: Set the permission for who may view the geo data associated with a
    photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.geo.setPerms
  tags: Photos,Geo,SetPerms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setperms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-geo-setperms-get-openapi.md
- name: Flickr Photos Licenses Get Info
  x-api-slug: flickr
  description: Fetches a list of available photo licenses for Flickr.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.licenses.getInfo
  tags: Photos,Licenses,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-licenses-getinfo-get-openapi.md
- name: Flickr Photos Licenses Set Info
  x-api-slug: flickr
  description: Sets the license for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.licenses.setInfo
  tags: Photos,Licenses,SetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-licenses-setinfo-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-licenses-setinfo-post-openapi.md
- name: Flickr Photos Notes Add
  x-api-slug: flickr
  description: Add a note to a photo. Coordinates and sizes are in pixels, based on
    the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.add
  tags: Photos,Notes,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-add-post-openapi.md
- name: Flickr Photos Notes Delete
  x-api-slug: flickr
  description: Delete a note from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.delete
  tags: Photos,Notes,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-delete-post-openapi.md
- name: Flickr Photos Notes Edit
  x-api-slug: flickr
  description: Edit a note on a photo. Coordinates and sizes are in pixels, based
    on the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.notes.edit
  tags: Photos,Notes,Edit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-edit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-notes-edit-post-openapi.md
- name: Flickr Photos People Add
  x-api-slug: flickr
  description: Add a person to a photo. Coordinates and sizes are in pixels, based
    on the 500px image size shown on individual photo pages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.add
  tags: Photos,People,Add
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-add-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-add-post-openapi.md
- name: Flickr Photos People Delete
  x-api-slug: flickr
  description: Remove a person from a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.delete
  tags: Photos,People,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-delete-post-openapi.md
- name: Flickr Photos People Delete Coords
  x-api-slug: flickr
  description: Remove the bounding box from a person in a photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.deleteCoords
  tags: Photos,People,DeleteCoords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-deletecoords-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-deletecoords-post-openapi.md
- name: Flickr Photos People Edit Coords
  x-api-slug: flickr
  description: Edit the bounding box of an existing person on a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.editCoords
  tags: Photos,People,EditCoords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-editcoords-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-editcoords-post-openapi.md
- name: Flickr Photos People Get List
  x-api-slug: flickr
  description: Get a list of people in a given photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.people.getList
  tags: Photos,People,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-people-getlist-get-openapi.md
- name: Flickr Photos Transform Rotate
  x-api-slug: flickr
  description: Rotate a photo.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.transform.rotate
  tags: Photos,Transform,Rotate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-transform-rotate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-transform-rotate-post-openapi.md
- name: Flickr Photos Upload Check Tickets
  x-api-slug: flickr
  description: Checks the status of one or more asynchronous photo upload tickets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.upload.checkTickets
  tags: Photos,Upload,CheckTickets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-upload-checktickets-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photos-upload-checktickets-get-openapi.md
- name: Flickr Photosets Add Photo
  x-api-slug: flickr
  description: Add a photo to the end of an existing photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.addPhoto
  tags: Photosets,AddPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-addphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-addphoto-post-openapi.md
- name: Flickr Photosets Create
  x-api-slug: flickr
  description: Create a new photoset for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.create
  tags: Photosets,Create
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-create-post-openapi.md
- name: Flickr Photosets Delete
  x-api-slug: flickr
  description: Delete a new photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.delete
  tags: Photosets,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-delete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-delete-post-openapi.md
- name: Flickr Photosets Edit Meta
  x-api-slug: flickr
  description: Modify the meta-data for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.editMeta
  tags: Photosets,EditMeta
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-editmeta-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-editmeta-post-openapi.md
- name: Flickr Photosets Edit Photos
  x-api-slug: flickr
  description: Modify the photos in a photoset. Use this method to add, remove and
    re-order photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.editPhotos
  tags: Photosets,EditPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-editphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-editphotos-post-openapi.md
- name: Flickr Photosets Get Context
  x-api-slug: flickr
  description: Returns next and previous photos for a photo in a set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getContext
  tags: Photosets,GetContext
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getcontext-get-openapi.md
- name: Flickr Photosets Get Info
  x-api-slug: flickr
  description: Gets information about a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getInfo
  tags: Photosets,GetInfo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getinfo-get-openapi.md
- name: Flickr Photosets Get List
  x-api-slug: flickr
  description: Returns the photosets belonging to the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getList
  tags: Photosets,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getlist-get-openapi.md
- name: Flickr Photosets Get Photos
  x-api-slug: flickr
  description: Get the list of photos in a set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.getPhotos
  tags: Photosets,GetPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-getphotos-get-openapi.md
- name: Flickr Photosets Order Sets
  x-api-slug: flickr
  description: Set the order of photosets for the calling user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.orderSets
  tags: Photosets,OrderSets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-ordersets-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-ordersets-post-openapi.md
- name: Flickr Photosets Remove Photo
  x-api-slug: flickr
  description: Remove a photo from a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.removePhoto
  tags: Photosets,RemovePhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-removephoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-removephoto-post-openapi.md
- name: Flickr Photosets Remove Photos
  x-api-slug: flickr
  description: Remove multiple photos from a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.removePhotos
  tags: Photosets,RemovePhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-removephotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-removephotos-post-openapi.md
- name: Flickr Photosets Reorder Photos
  x-api-slug: flickr
  description: Update the order of photos in a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.reorderPhotos
  tags: Photosets,ReorderPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-reorderphotos-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-reorderphotos-post-openapi.md
- name: Flickr Photosets Set Primary Photo
  x-api-slug: flickr
  description: Set photoset primary photo
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.setPrimaryPhoto
  tags: Photosets,SetPrimaryPhoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-setprimaryphoto-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-setprimaryphoto-post-openapi.md
- name: Flickr Photosets Comments Add Comment
  x-api-slug: flickr
  description: Add a comment to a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.addComment
  tags: Photosets,Comments,AddComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-addcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-addcomment-post-openapi.md
- name: Flickr Photosets Comments Delete Comment
  x-api-slug: flickr
  description: Delete a photoset comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.deleteComment
  tags: Photosets,Comments,DeleteComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-deletecomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-deletecomment-post-openapi.md
- name: Flickr Photosets Comments Edit Comment
  x-api-slug: flickr
  description: Edit the text of a comment as the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.editComment
  tags: Photosets,Comments,EditComment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-editcomment-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-editcomment-post-openapi.md
- name: Flickr Photosets Comments Get List
  x-api-slug: flickr
  description: Returns the comments for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photosets.comments.getList
  tags: Photosets,Comments,GetList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-getlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-photosets-comments-getlist-get-openapi.md
- name: Flickr Places Get Children With Photos Public
  x-api-slug: flickr
  description: Return a list of locations with public photos that are parented by
    a Where on Earth (WOE) or Places ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getChildrenWithPhotosPublic
  tags: Places,GetChildrenWithPhotosPublic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-openapi.md
- name: Flickr Stats Get Photo Stats
  x-api-slug: flickr
  description: Get the number of views, comments and favorites on a photo for a given
    date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotoStats
  tags: Stats,GetPhotoStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostats-get-openapi.md
- name: Flickr Stats Get Photoset Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetDomains
  tags: Stats,GetPhotosetDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetdomains-get-openapi.md
- name: Flickr Stats Get Photoset Referrers
  x-api-slug: flickr
  description: Get a list of referring domains for a photoset.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetReferrers
  tags: Stats,GetPhotosetReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetreferrers-get-openapi.md
- name: Flickr Stats Get Photoset Stats
  x-api-slug: flickr
  description: Get the number of views on a photoset for a given date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotosetStats
  tags: Stats,GetPhotosetStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotosetstats-get-openapi.md
- name: Flickr Stats Get Photostream Domains
  x-api-slug: flickr
  description: Get a list of referring domains for a photostream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamDomains
  tags: Stats,GetPhotostreamDomains
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamdomains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamdomains-get-openapi.md
- name: Flickr Stats Get Photostream Referrers
  x-api-slug: flickr
  description: Get a list of referrers from a given domain to a user's photostream
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamReferrers
  tags: Stats,GetPhotostreamReferrers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamreferrers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamreferrers-get-openapi.md
- name: Flickr Stats Get Photostream Stats
  x-api-slug: flickr
  description: Get the number of views on a user's photostream for a given date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPhotostreamStats
  tags: Stats,GetPhotostreamStats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getphotostreamstats-get-openapi.md
- name: Flickr Stats Get Popular Photos
  x-api-slug: flickr
  description: List the photos with the most views, comments or favorites.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.stats.getPopularPhotos
  tags: Stats,GetPopularPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getpopularphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-stats-getpopularphotos-get-openapi.md
- name: Flickr Tags Get Cluster Photos
  x-api-slug: flickr
  description: Returns the first 24 photos for a given tag cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.tags.getClusterPhotos
  tags: Tags,GetClusterPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-tags-getclusterphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-tags-getclusterphotos-get-openapi.md
- name: Flickr Urls Get User Photos
  x-api-slug: flickr
  description: Returns the url to a user's photos.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.urls.getUserPhotos
  tags: Urls,GetUserPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-urls-getuserphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/restmethodflickr-urls-getuserphotos-get-openapi.md
- name: Flickr
  x-api-slug: flickr
  description: The Flickr API consists of a set of callable methods, and some API
    endpoints.  To perform an action using the Flickr API, you need to select a calling
    convention, send a request to its endpoint specifying a method and some arguments,
    and will receive a formatted response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services/
  tags: Photos
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/flickr/openapi.md
x-common:
- type: x-authentication
  url: https://www.flickr.com/services/api/auth.oauth.html
- type: x-base
  url: https://api.flickr.com/services/
- type: x-developer
  url: https://www.flickr.com/services/api/
- type: x-getting-started
  url: https://www.flickr.com/services/developer/
- type: x-privacy
  url: https://info.yahoo.com/privacy/us/yahoo/flickr/details.html
- type: x-support
  url: https://help.yahoo.com/kb/flickr-for-desktop
- type: x-terms-of-service
  url: https://www.flickr.com/services/api/tos/
- type: x-twitter
  url: https://twitter.com/flickr
- type: x-website
  url: http://www.flickr.com/
- type: x-website
  url: http://flickr.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---