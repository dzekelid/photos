---
swagger: "2.0"
info:
  title: Flickr
  version: 1.0.0
host: api.flickr.com
basePath: /services
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest?method=flickr.photos.search:
    get:
      summary: Photo Search
      description: Return a list of photos matching some criteria
      operationId: getMediaBySearch
      parameters:
      - in: query
        name: accuracy
        description: Recorded accuracy level of the location information
      - in: query
        name: api_key
      - in: query
        name: bbox
        description: A comma-delimited list of 4 values defining the Bounding Box
          of the area that will be searched
      - in: query
        name: contacts
        description: Search your contacts
      - in: query
        name: content_type
        description: |-
          Content Type setting:
            1: photos only
      - in: query
        name: geo_context
        description: Geo context is a numeric value representing the photo's geotagginess
          beyond latitude and longitude
      - in: query
        name: group_id
        description: The id of a group who's pool to search
      - in: query
        name: has_geo
        description: Any photo that has been geotagged, or if the value is "0" any
          photo that has not been geotagged
      - in: query
        name: in_gallery
        description: Limit the scope of the search to only photos that are in a gallery?
          Default is false, search all photos
      - in: query
        name: is_commons
        description: Limit the scope of the search to only photos that are part of
          the Flickr Commons project
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
        description: 'Aside from passing in a fully formed machine tag, there is a
          special syntax for searching on specific properties : Find photos using
          the ''dc'' namespace : "machine_tags" => "dc:" Find photos with a title
          in the ''dc'' namespace : "machine_tags" => "dc:title=" Find photos titled
          "mr'
      - in: query
        name: machine_tag_mode
        description: Either 'any' for an OR combination of tags, or 'all' for an AND
          combination
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
        description: |
          Safe search setting:
            1: for safe,
            2: for moderate,
            3: for restricted
      - in: query
        name: sort
        description: The order in which to sort returned photos
      - in: query
        name: tags
        description: A comma-delimited list of tags
      - in: query
        name: text
        description: A free text search
      - in: query
        name: user_id
        description: The NSID of the user who's photo to search
      - in: query
        name: woe_id
        description: A 32-bit identifier that uniquely represents spatial entities
      responses:
        200:
          description: OK
      tags:
      - photos
definitions:
  ContextPhoto:
    properties:
      id:
        description: This is a default description.
        type: post
      secret:
        description: This is a default description.
        type: post
      server:
        description: This is a default description.
        type: post
      farm:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
      thumb:
        description: This is a default description.
        type: post
      media:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      license:
        description: This is a default description.
        type: post
  ContextPhotos:
    properties:
      photos:
        description: This is a default description.
        type: post
  Cover:
    properties:
      id:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      secret:
        description: This is a default description.
        type: post
      server:
        description: This is a default description.
        type: post
      farm:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
      ispublic:
        description: This is a default description.
        type: post
      isfriend:
        description: This is a default description.
        type: post
      isfamily:
        description: This is a default description.
        type: post
      "y":
        description: This is a default description.
        type: post
  Group:
    properties:
      id:
        description: This is a default description.
        type: post
      path_alias:
        description: This is a default description.
        type: post
      iconserver:
        description: This is a default description.
        type: post
      iconfarm:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      members:
        description: This is a default description.
        type: post
      pool_count:
        description: This is a default description.
        type: post
      topic_count:
        description: This is a default description.
        type: post
  Note:
    properties:
      description:
        description: This is a default description.
        type: post
  Owner:
    properties:
      nsid:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
      realname:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      iconserver:
        description: This is a default description.
        type: post
      iconfarm:
        description: This is a default description.
        type: post
      path_alias:
        description: This is a default description.
        type: post
      noindexfollow:
        description: This is a default description.
        type: post
      ispro:
        description: This is a default description.
        type: post
      is_ad_free:
        description: This is a default description.
        type: post
  Person:
    properties:
      id:
        description: This is a default description.
        type: post
      nsid:
        description: This is a default description.
        type: post
      ispro:
        description: This is a default description.
        type: post
      can_buy_pro:
        description: This is a default description.
        type: post
      iconserver:
        description: This is a default description.
        type: post
      iconfarm:
        description: This is a default description.
        type: post
      path_alias:
        description: This is a default description.
        type: post
      has_stats:
        description: This is a default description.
        type: post
      coverphoto_server:
        description: This is a default description.
        type: post
      coverphoto_farm:
        description: This is a default description.
        type: post
  Photo:
    properties:
      id:
        description: This is a default description.
        type: post
      secret:
        description: This is a default description.
        type: post
      server:
        description: This is a default description.
        type: post
      farm:
        description: This is a default description.
        type: post
      dateuploaded:
        description: This is a default description.
        type: post
      isfavorite:
        description: This is a default description.
        type: post
      license:
        description: This is a default description.
        type: post
      safety_level:
        description: This is a default description.
        type: post
      rotation:
        description: This is a default description.
        type: post
      originalsecret:
        description: This is a default description.
        type: post
  PhotoURLs:
    properties:
      h:
        description: This is a default description.
        type: post
      l:
        description: This is a default description.
        type: post
      s:
        description: This is a default description.
        type: post
      t:
        description: This is a default description.
        type: post
  Tag:
    properties:
      id:
        description: This is a default description.
        type: post
      author:
        description: This is a default description.
        type: post
      authorname:
        description: This is a default description.
        type: post
      raw:
        description: This is a default description.
        type: post
      _content:
        description: This is a default description.
        type: post
      machine_tag:
        description: This is a default description.
        type: post
  Topic:
    properties:
      id:
        description: This is a default description.
        type: post
      subject:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
      author:
        description: This is a default description.
        type: post
      authorname:
        description: This is a default description.
        type: post
      author_path_alias:
        description: This is a default description.
        type: post
      author_is_deleted:
        description: This is a default description.
        type: post
      is_pro:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
      iconserver:
        description: This is a default description.
        type: post
  TopicReply:
    properties:
      id:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
      author:
        description: This is a default description.
        type: post
      authorname:
        description: This is a default description.
        type: post
      author_path_alias:
        description: This is a default description.
        type: post
      author_is_deleted:
        description: This is a default description.
        type: post
      is_pro:
        description: This is a default description.
        type: post
      iconserver:
        description: This is a default description.
        type: post
      iconfarm:
        description: This is a default description.
        type: post
      can_edit:
        description: This is a default description.
        type: post
  URL:
    properties:
      type:
        description: This is a default description.
        type: post
      _content:
        description: This is a default description.
        type: post
  Album:
    properties:
      id:
        description: This is a default description.
        type: post
      primary:
        description: This is a default description.
        type: post
      secret:
        description: This is a default description.
        type: post
      server:
        description: This is a default description.
        type: post
      farm:
        description: This is a default description.
        type: post
      photos:
        description: This is a default description.
        type: post
      videos:
        description: This is a default description.
        type: post
      count_views:
        description: This is a default description.
        type: post
      count_comments:
        description: This is a default description.
        type: post
      can_comment:
        description: This is a default description.
        type: post
x-collection-name: Flickr
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