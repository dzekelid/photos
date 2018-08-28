---
name: Plivo
x-slug: plivo
description: 'Voice & SMS API Platform: Plivo enables businesses and developers to
  tap into powerful Voice and SMS capabilities without carrier lock-in.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
x-kinRank: "8"
x-alexaRank: "130970"
tags: Photos
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/apis.md
specificationVersion: "0.14"
apis:
- name: Codenvy Account API - Post Photos
  x-api-slug: photos-post
  description: Create a new photo on behalf of the user, and receive an upload key
    in exchange.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photos-post-openapi.md
- name: Codenvy Account API - Put Photos
  x-api-slug: photosid-put
  description: 'Allows the client application to update user-editable information
    on a photo.nnnResource URLnnhttps://api.500px.com/v1/photos/:idnnnnAuthenticationnnRequired;
    OAuth. The client application must use the OAuth access token issued for the owner
    of the photo to access this resouce.nnnParametersnnThe application must provide
    the ID of the photo to update in the URL of the request. The following parameters
    are recognized when included in the query string or POST body:nnnnname: Title
    of the photo, up to 255 characters in length.nndescription: Text description of
    the photo, up to 65535 characters in length.nncategory: Integer number of the
    category of the photo. See category mapping for exact values.nntags: Comma-separated
    list of tags applicable to this photo.nnadd_tags: Comma-separated list of tags
    to add to this photos existing tags.nnremove_tags: Comma-separated list of tags
    to remove from this photos existing tags.nnshutter_speed: Shutter speed value
    for the photo, internally stored as string.nnfocal_length: Focal length value
    for the photo, internally stored as string.nnaperture: Aperture value value for
    the photo, internally stored as string.nniso: Integer ISO value for the photo.nncamera:
    Make and model of the camera used to take this photo.nnlens: Information about
    the lens used to take this photo.nnlatitude: Latitude of the location this photo
    was taken at represented by a decimal number.nnlongitude: Longitude of the location
    this photo was taken at represented by a decimal number.nnnsfw: Boolean value
    indicating that the photo may contain not-safe-for-work content or content not
    suitable for minors.nnlicense_type: Integer number of the license type chosen
    for this photo. See license type mapping for exact values.nnprivacy: Integer value
    indicating that the photo should be shown (0) or hidden (1) on the users profile.nncrop:
    A hash containing keys x, x2, y, y2 and representing coordinates within which
    the thumbnail must be cropped. The crop is made using the top left corner as the
    origin. The points must be given relative to image size 4, an image of at most
    900px on the larger side. The client application may skip this if the user does
    not wish to change photo thumbnail.nnnnImplementation detailsnnA parameter missing
    from the request will not be updated.  A parameter set to an empty string or null
    value will be interpreted as the user wishing to reset the value of the field
    to its default value.nnYou can use the add_tags and remove_tags parameters to
    manupulate a photos tags without having to send the complete list of tags in the
    request.nnnReturn formatnnA JSON object containing key photo, where photo is a
    Photo object in full format.nnnErrorsnnAll known errors cause the resource to
    return HTTP error code header together with a JSON array containing at least status
    and error keys describing the source of error.nnnn401: Invalid OAuth request:
    The request was refused because the OAuth signature is incorrect.nn404: Photo
    with ID not found: The photo ID provided is not known to the system.nn404: Photo
    with ID has been deleted: The photo has been deleted and can not be edited.nn404:
    Photo with ID belongs to a deactivated user: The photo belongs to a user that
    is no longer active and can not be edited.nn400: Bad photo category: An unrecognized
    photo category value has been provided.nn400: Bad license type: An unrecognized
    license type value has been provided.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosid-put-openapi.md
- name: Codenvy Account API - Post Photos Comments
  x-api-slug: photosidcomments-post
  description: Creates a new comment for the photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidcomments-post-openapi.md
- name: Codenvy Account API - Post Photos Favorite
  x-api-slug: photosidfavorite-post
  description: Adds the photo to users list of favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidfavorite-post-openapi.md
- name: Codenvy Account API - Get Photos Favorites
  x-api-slug: photosidfavorites-get
  description: Returns all users that had favorite that photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidfavorites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidfavorites-get-openapi.md
- name: Codenvy Account API - Post Photos Report
  x-api-slug: photosidreport-post
  description: Allows to report a photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidreport-post-openapi.md
- name: Codenvy Account API - Post Photos Tags
  x-api-slug: photosidtags-post
  description: Adds tags to the photo. Accepts one or multiple coma separated tags.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidtags-post-openapi.md
- name: Codenvy Account API - Post Photos Vote
  x-api-slug: photosidvote-post
  description: Allows the user to vote for a photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidvote-post-openapi.md
- name: Codenvy Account API - Get Photos Votes
  x-api-slug: photosidvotes-get
  description: Returns all users that had liked this photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosidvotes-get-openapi.md
- name: Codenvy Account API - Get Photos Search
  x-api-slug: photossearch-get
  description: Returns a listing of twenty (up to one hundred) photos from search
    results for a specified tag, keyword, or location.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photossearch-get-openapi.md
- name: Codenvy Account API - Post Photos Upload
  x-api-slug: photosupload-post
  description: This is a new photo upload endpoint. It is currently in beta.nCreate
    a new photo on behalf of the user and upload a file.nfile parameter is passed
    in multipart/form-data, other parameters are passed as query parametrs or multipart/form-data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1113-plivo.jpg
  humanURL: http:///account
  baseURL: :///account/https://codenvy.com/api
  tags: Voice, Target, Imports, Stack Network, Technology, Telecommunications, SMS,
    Telecommunications, Messages, Relative Data, Service API, Relative StreamRank,
    Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/plivo/photosupload-post-openapi.md
x-common:
- type: x--net-library
  url: https://www.plivo.com/docs/helpers/dotnet/
- type: x-android-sdk
  url: https://www.plivo.com/docs/sdk/android/
- type: x-api-gallery
  url: http://plentymarkets.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plivo.stack.network
- type: x-base
  url: https://api.plivo.com
- type: x-blog
  url: http://blog.plivo.com
- type: x-blog-rss
  url: http://blog.plivo.com/rss
- type: x-crunchbase
  url: https://crunchbase.com/organization/plivo
- type: x-crunchbase
  url: http://www.crunchbase.com/company/plivo
- type: x-documentation
  url: https://plivo.com/docs/
- type: x-email
  url: marketing@plivo.com
- type: x-email
  url: legalrequests@plivo.com
- type: x-email
  url: privacy@plivo.com
- type: x-faq
  url: https://plivo.com/faq/
- type: x-github
  url: https://github.com/plivo
- type: x-ios-sdk
  url: https://www.plivo.com/docs/sdk/ios/
- type: x-java-sdk
  url: https://www.plivo.com/docs/helpers/java/
- type: x-linkedin
  url: https://www.linkedin.com/company/plivo-inc/
- type: x-node-js-library
  url: https://www.plivo.com/docs/helpers/node/
- type: x-php-sdk
  url: https://www.plivo.com/docs/helpers/php/
- type: x-pricing
  url: https://plivo.com/pricing/
- type: x-privacy
  url: https://plivo.com/privacy/
- type: x-ruby-library
  url: https://www.plivo.com/docs/helpers/python
- type: x-selfservice-registration
  url: https://manage.plivo.com/accounts/register/
- type: x-status
  url: https://status.plivo.com/
- type: x-terms-of-service
  url: https://plivo.com/terms/
- type: x-twitter
  url: https://twitter.com/plivo
- type: x-website
  url: http:///account
- type: x-website
  url: http://plivo.com
- type: x-website
  url: https://www.plivo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---