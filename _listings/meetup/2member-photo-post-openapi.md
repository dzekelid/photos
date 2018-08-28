---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Member Photo Upload
  description: Uploads a photo to be associated with a Member
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /photos:
    get:
      summary: Photos
      description: API method for accessing meetup photos
      operationId: deprecated
      x-api-path-slug: photos-get
      parameters:
      - in: query
        name: album_id
        description: return photos for the albums with the given id, separated by
          commas
        type: string
      - in: query
        name: group_id
        description: Return photos in groups with these ID numbers [separated by commas]
        type: string
      - in: query
        name: group_urlname
        description: return photos for the group with given custom URL path
        type: string
      - in: query
        name: topic
        description: Return photos in this topic
        type: string
      - in: query
        name: topic, groupnum
        description: return photos for the group with given topic and number
        type: string
      - in: query
        name: topic_id
        description: Return photos in topics with this ID number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /2/photo/:id:
    delete:
      summary: Event Photo Delete
      description: Deletes a specified event photo
      operationId: photos
      x-api-path-slug: 2photoid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    post:
      summary: Event Photo Edit
      description: Edits a specified event photo
      operationId: photos
      x-api-path-slug: 2photoid-post
      parameters:
      - in: query
        name: caption
        description: Photo caption of up to 255 characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /2/photo_comment:
    post:
      summary: Photo Comment v2
      description: This method posts comments that appear below photos
      operationId: photos
      x-api-path-slug: 2photo-comment-post
      parameters:
      - in: query
        name: comment
        description: The comment text
        type: string
      - in: query
        name: photo_id
        description: The photo related to this comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /2/photo_albums:
    get:
      summary: Photo Albums
      description: This method returns photo albums associated with Meetup groups.
        To create albums, see the corresponding write method.
      operationId: photos
      x-api-path-slug: 2photo-albums-get
      parameters:
      - in: query
        name: event_id
        description: Return photo albums for these event ids, separated by commas
        type: string
      - in: query
        name: group_id
        description: Return albums in groups with these ID, separated by commas
        type: string
      - in: query
        name: photo_album_id
        description: Return albums with these IDs, separated by commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /2/photos:
    get:
      summary: Photos
      description: This method returns photos by member, group, album, event, photo
        ID, or tagged member.
      operationId: photos
      x-api-path-slug: 2photos-get
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: callback
        description: Name of a function to be called with an array of photo notification
          objects
        type: string
      - in: query
        name: event_id
        description: Limit notifications to a specific event id
        type: string
      - in: query
        name: event_id
        description: Event ids, separated by commas
        type: string
      - in: query
        name: fields
        description: comma-delimited optional response properties such as member_country,
          member_city, member_state, and self
        type: string
      - in: query
        name: group_id
        description: Group IDs, separated by commas
        type: string
      - in: query
        name: group_urlname
        description: Group urlnames, separated by commas
        type: string
      - in: query
        name: member_id
        description: Uploaded by members with these IDs, separated by commas
        type: string
      - in: query
        name: photo_album_id
        description: Photo Album IDs, separated by commas
        type: string
      - in: query
        name: photo_id
        description: Photo IDs, separated by commas
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Should be supplied for all but the first polling request, so
          that any missed notifications are can be sent in an immediate response
        type: string
      - in: query
        name: tagged
        description: Tagged with members with these IDs, separated by commas
        type: string
      - in: query
        name: time
        description: Return photos uploaded within the given time range, defined by
          two times separated with a single comma
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    ws:
      summary: WebSocket Photo Stream
      description: |-
        For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
        efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
        any messages received from the client after the socket is open.

        Because browser support for WebSockets is limited, we recommend that you consume this stream
        through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
      operationId: streams
      x-api-path-slug: 2photos-ws
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent photos with an mtime greater then the supplied
          time, in millisends since the epoch
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Albums
  /2/photo_album:
    post:
      summary: Photo Album2
      description: This method creates photo albums within a Meetup group
      operationId: photos
      x-api-path-slug: 2photo-album-post
      parameters:
      - in: query
        name: group_id
        description: Group to create the album in
        type: string
      - in: query
        name: title
        description: Title of the new album
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Albums
  /2/open_venues:
    get:
      summary: OpenVenues
      description: Searches for public venues within a given geo space. To search
        for specific venues that your group has used, use the [Venues](/meetup_api/docs/2/venues)
        method
      operationId: venues
      x-api-path-slug: 2open-venues-get
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: city
        description: A valid city
        type: string
      - in: query
        name: country
        description: A valid country code
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_urlname
        description: Returns venues with location relative to the group associated
          with this urlname
        type: string
      - in: query
        name: lat
        description: A valid latitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: lon
        description: A valid longitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: radius
        description: Radius, in miles for geographic requests, default 25
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent open venues with an mtime greater then the supplied
          time, in milliseconds since the epoch
        type: string
      - in: query
        name: state
        description: For the US, a valid 2 character state code
        type: string
      - in: query
        name: text
        description: Venues that contain the given term or terms somewhere in their
          content
        type: string
      - in: query
        name: trickle
        description: When supplied with a request, the Meetup API will push your client
          the entire Meetup database of public venues in batches of 512
        type: string
      - in: query
        name: zip
        description: A valid US zip code, limits the returned venues to those within
          radius miles
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /2/photo:
    post:
      summary: Event Photo Upload
      description: Uploads a photo for a given event
      operationId: photos
      x-api-path-slug: 2photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: caption
        description: Caption for the photo
        type: string
      - in: query
        name: event_id
        description: Identifier of an event
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: photo_album_id
        description: Identifier of an existing photo album, which may be an event
          or group album
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/venues:
    get:
      summary: Group Venues
      description: Returns venues a group has previously hosted events at
      operationId: venues
      x-api-path-slug: urlnamevenues-get
      parameters:
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Veues
    post:
      summary: Venue Create
      description: Interface for creating new Meetup venues
      operationId: venues
      x-api-path-slug: urlnamevenues-post
      parameters:
      - in: query
        name: address_1
        description: Primary address of the venue
        type: string
      - in: query
        name: address_2
        description: Secondary address info
        type: string
      - in: query
        name: city
        description: City name of the venue
        type: string
      - in: query
        name: country
        description: 2 character country code of the venue
        type: string
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: hours
        description: Open hours information about the venue
        type: string
      - in: query
        name: name
        description: Unique name of the venue
        type: string
      - in: query
        name: phone
        description: Optional phone number for the venue
        type: string
      - in: query
        name: state
        description: If in the US or CA, the state code for the venue
        type: string
      - in: query
        name: visibility
        description: Optional value indicating the venues visibility to others
        type: string
      - in: query
        name: web_url
        description: Optional web url for the venue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Veues
  /:urlname/events/:event_id/hosts:
    get:
      summary: Event Hosts
      description: Returns the list of hosts for a given event
      operationId: hosts
      x-api-path-slug: urlnameeventsevent-idhosts-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums/:album_id/photos:
    get:
      summary: Album Photos
      description: Lists photos for a given photo album
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-idphotos-get
      parameters:
      - in: query
        name: desc
        description: Controls directional order or listing
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: page
        description: Number of items to return per-page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    post:
      summary: Album Photo Upload
      description: Support for uploading new Album photos
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-idphotos-post
      parameters:
      - in: query
        name: await
        description: Optional boolean parameter that will defer a requests a response
          until confirmation that photo is immediately displayable is received
        type: string
      - in: query
        name: caption
        description: Caption for display
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: photo
        description: Photo upload data, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/events/:event_id/photos:
    get:
      summary: Event Photos
      description: Lists photos for a given event
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotos-get
      parameters:
      - in: query
        name: desc
        description: Controls directional order or listing
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: page
        description: Number of items to return per-page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    post:
      summary: Event Photo Upload
      description: Support for uploading new Event photos
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotos-post
      parameters:
      - in: query
        name: await
        description: Optional boolean parameter that will defer a requests a response
          until confirmation that photo is immediately displayable is received
        type: string
      - in: query
        name: caption
        description: Caption for display
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: photo
        description: Photo upload data, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/events/:event_id/photos/:photo_id:
    get:
      summary: Event Photo
      description: Gets information about a specific photo
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    patch:
      summary: Event Photo Edit
      description: Edits photo details
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-id-patch
      parameters:
      - in: query
        name: caption
        description: The photo caption
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    delete:
      summary: Event Photo Delete
      description: Deletes a specified event photo
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photos:
    get:
      summary: Album Photos
      description: Lists of all photos uploaded for the group
      operationId: photos
      x-api-path-slug: urlnamephotos-get
      parameters:
      - in: query
        name: desc
        description: Controls directional order or listing
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: page
        description: Number of items to return per-page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/topics:
    post:
      summary: Group Topics Add
      description: Associates topics with a given Meetup group. Limited to organizers
        of the group. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
        permission.
      operationId: groups
      x-api-path-slug: urlnametopics-post
      parameters:
      - in: query
        name: topic_id
        description: Comma-delimited list of topic ids to associate with group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
    delete:
      summary: Group Topics Remove
      description: Disassociates topics with a given Meetup group. Limited to organizers
        of the group. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
        permission.
      operationId: groups
      x-api-path-slug: urlnametopics-delete
      parameters:
      - in: query
        name: topic_id
        description: Comma-delimited list of topic ids to disassociate with group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /members/:member_id/photos/:photo_id:
    delete:
      summary: Member Photo Delete
      description: Deletes a member photo by id
      operationId: photos
      x-api-path-slug: membersmember-idphotosphoto-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /members/:member_id/photos:
    post:
      summary: Member Photo Upload
      description: Support for uploading new Member photos
      operationId: photos
      x-api-path-slug: membersmember-idphotos-post
      parameters:
      - in: query
        name: await
        description: Optional boolean parameter that, when set to true, will defer
          a requests a response until confirmation that photo is immediately displayable
          is received
        type: string
      - in: query
        name: main
        description: Optional boolean parameter that, when set to true, will cause
          the members main profile photo to be set to the uploaded photo
        type: string
      - in: query
        name: photo
        description: Photo upload data, encoded as a multipart/form-data file
        type: string
      - in: query
        name: sync_photo
        description: Optional boolean parameter that, when set to true, will sync
          all of the group profile photos for the member with the provided photo
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums/:album_id:
    get:
      summary: Photo Album
      description: Gets information about a specific photo album
      operationId: photos
      x-api-path-slug: urlnamephoto-albumsalbum-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/photo_albums:
    get:
      summary: Photo Album List
      description: Gets a list a group photo albums in ascending order based on the
        time they were created
      operationId: photos
      x-api-path-slug: urlnamephoto-albums-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional response fields
        type: string
      - in: query
        name: offset
        description: Incrementing number used for pagination offsets
        type: string
      - in: query
        name: page
        description: Number of albums to return per page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/events/:event_id/photos/:photo_id/comments:
    post:
      summary: Photo Comment
      description: Creates a new photo comment
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-idcomments-post
      parameters:
      - in: query
        name: comment
        description: The text of the comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
    get:
      summary: Photo Comments
      description: Lists photo comments associated with a photo
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-idcomments-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /:urlname/events/:event_id/photos/:photo_id/comments/:comment_id:
    delete:
      summary: Photo Comment Delete
      description: Deletes photo comments
      operationId: photos
      x-api-path-slug: urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Comments
  /:urlname/similar_groups:
    get:
      summary: Similar groups
      description: Renders a list of similar groups
      operationId: groups
      x-api-path-slug: urlnamesimilar-groups-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /2/group_photo:
    post:
      summary: Group Photo Upload
      description: Uploads a new Meetup Group photo. To change other Group settings
        use the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
      operationId: groups
      x-api-path-slug: 2group-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: group_id
        description: Group ID for the target group
        type: string
      - in: query
        name: group_urlname
        description: Group urlname
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the groups main photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /2/member_photo:
    post:
      summary: Member Photo Upload
      description: Uploads a photo to be associated with a Member
      operationId: members
      x-api-path-slug: 2member-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the members main profile
          photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: sync_matching_photo
        description: When set to true and main is set to true, this will replace all
          group profile photos matching the current photo with the provided replacement
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
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