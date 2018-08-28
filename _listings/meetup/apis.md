---
name: Meetup
x-slug: meetup
description: Find Meetups so you can do more of what matters to you. Or create your
  own group and meet people near you who share your interests.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
x-kinRank: "9"
x-alexaRank: "917"
tags: Photos
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup - Photos
  x-api-slug: photos-get
  description: API method for accessing meetup photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/photos-get-openapi.md
- name: Meetup - Event Photo Delete
  x-api-slug: 2photoid-delete
  description: Deletes a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photoid-delete-openapi.md
- name: Meetup - Event Photo Edit
  x-api-slug: 2photoid-post
  description: Edits a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photoid-post-openapi.md
- name: Meetup - Photo Comment v2
  x-api-slug: 2photo-comment-post
  description: This method posts comments that appear below photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-comment-post-openapi.md
- name: Meetup - Photo Albums
  x-api-slug: 2photo-albums-get
  description: This method returns photo albums associated with Meetup groups. To
    create albums, see the corresponding write method.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-albums-get-openapi.md
- name: Meetup - Photos
  x-api-slug: 2photos-get
  description: This method returns photos by member, group, album, event, photo ID,
    or tagged member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photos-get-openapi.md
- name: Meetup - Photo Album2
  x-api-slug: 2photo-album-post
  description: This method creates photo albums within a Meetup group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-album-post-openapi.md
- name: Meetup - OpenVenues
  x-api-slug: 2open-venues-get
  description: Searches for public venues within a given geo space. To search for
    specific venues that your group has used, use the [Venues](/meetup_api/docs/2/venues)
    method
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2open-venues-get-openapi.md
- name: Meetup - Event Photo Upload
  x-api-slug: 2photo-post
  description: Uploads a photo for a given event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-post-openapi.md
- name: Meetup - WebSocket Photo Stream
  x-api-slug: 2photos-ws
  description: |-
    For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
    efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
    any messages received from the client after the socket is open.

    Because browser support for WebSockets is limited, we recommend that you consume this stream
    through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photos-ws-openapi.md
- name: Meetup - Group Venues
  x-api-slug: urlnamevenues-get
  description: Returns venues a group has previously hosted events at
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamevenues-get-openapi.md
- name: Meetup - Venue Create
  x-api-slug: urlnamevenues-post
  description: Interface for creating new Meetup venues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamevenues-post-openapi.md
- name: Meetup - Event Hosts
  x-api-slug: urlnameeventsevent-idhosts-get
  description: Returns the list of hosts for a given event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idhosts-get-openapi.md
- name: Meetup - Album Photos
  x-api-slug: urlnamephoto-albumsalbum-idphotos-get
  description: Lists photos for a given photo album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-idphotos-get-openapi.md
- name: Meetup - Album Photo Upload
  x-api-slug: urlnamephoto-albumsalbum-idphotos-post
  description: Support for uploading new Album photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-idphotos-post-openapi.md
- name: Meetup - Event Photos
  x-api-slug: urlnameeventsevent-idphotos-get
  description: Lists photos for a given event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotos-get-openapi.md
- name: Meetup - Event Photo
  x-api-slug: urlnameeventsevent-idphotosphoto-id-get
  description: Gets information about a specific photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-get-openapi.md
- name: Meetup - Event Photo Edit
  x-api-slug: urlnameeventsevent-idphotosphoto-id-patch
  description: Edits photo details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-patch-openapi.md
- name: Meetup - Event Photo Delete
  x-api-slug: urlnameeventsevent-idphotosphoto-id-delete
  description: Deletes a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-delete-openapi.md
- name: Meetup - Event Photo Upload
  x-api-slug: urlnameeventsevent-idphotos-post
  description: Support for uploading new Event photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotos-post-openapi.md
- name: Meetup - Album Photos
  x-api-slug: urlnamephotos-get
  description: Lists of all photos uploaded for the group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephotos-get-openapi.md
- name: Meetup - Group Topics Add
  x-api-slug: urlnametopics-post
  description: Associates topics with a given Meetup group. Limited to organizers
    of the group. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
    permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnametopics-post-openapi.md
- name: Meetup - Group Topics Remove
  x-api-slug: urlnametopics-delete
  description: Disassociates topics with a given Meetup group. Limited to organizers
    of the group. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
    permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnametopics-delete-openapi.md
- name: Meetup - Member Photo Delete
  x-api-slug: membersmember-idphotosphoto-id-delete
  description: Deletes a member photo by id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/membersmember-idphotosphoto-id-delete-openapi.md
- name: Meetup - Member Photo Upload
  x-api-slug: membersmember-idphotos-post
  description: Support for uploading new Member photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/membersmember-idphotos-post-openapi.md
- name: Meetup - Photo Album
  x-api-slug: urlnamephoto-albumsalbum-id-get
  description: Gets information about a specific photo album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-id-get-openapi.md
- name: Meetup - Photo Album List
  x-api-slug: urlnamephoto-albums-get
  description: Gets a list a group photo albums in ascending order based on the time
    they were created
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albums-get-openapi.md
- name: Meetup - Photo Comment
  x-api-slug: urlnameeventsevent-idphotosphoto-idcomments-post
  description: Creates a new photo comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-post-openapi.md
- name: Meetup - Photo Comment Delete
  x-api-slug: urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete
  description: Deletes photo comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete-openapi.md
- name: Meetup - Photo Comments
  x-api-slug: urlnameeventsevent-idphotosphoto-idcomments-get
  description: Lists photo comments associated with a photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-get-openapi.md
- name: Meetup - Similar groups
  x-api-slug: urlnamesimilar-groups-get
  description: Renders a list of similar groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamesimilar-groups-get-openapi.md
- name: Meetup - Group Photo Upload
  x-api-slug: 2group-photo-post
  description: Uploads a new Meetup Group photo. To change other Group settings use
    the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2group-photo-post-openapi.md
- name: Meetup - Member Photo Upload
  x-api-slug: 2member-photo-post
  description: Uploads a photo to be associated with a Member
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2member-photo-post-openapi.md
- name: Meetup - Member Photo Delete
  x-api-slug: 2member-photoid-delete
  description: Delete the specified member photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2member-photoid-delete-openapi.md
- name: Meetup - Event Photo Upload
  x-api-slug: 2photo-post
  description: Uploads a photo for a given event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-post-openapi.md
- name: Meetup - Event Photo Delete
  x-api-slug: 2photoid-delete
  description: Deletes a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photoid-delete-openapi.md
- name: Meetup - Event Photo Edit
  x-api-slug: 2photoid-post
  description: Edits a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photoid-post-openapi.md
- name: Meetup - Photos
  x-api-slug: 2photos-get
  description: This method returns photos by member, group, album, event, photo ID,
    or tagged member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photos-get-openapi.md
- name: Meetup - WebSocket Photo Stream
  x-api-slug: 2photos-ws
  description: |-
    For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
    efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
    any messages received from the client after the socket is open.

    Because browser support for WebSockets is limited, we recommend that you consume this stream
    through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photos-ws-openapi.md
- name: Meetup - Photo Album2
  x-api-slug: 2photo-album-post
  description: This method creates photo albums within a Meetup group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-album-post-openapi.md
- name: Meetup - Photo Albums
  x-api-slug: 2photo-albums-get
  description: This method returns photo albums associated with Meetup groups. To
    create albums, see the corresponding write method.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-albums-get-openapi.md
- name: Meetup - Photo Comment v2
  x-api-slug: 2photo-comment-post
  description: This method posts comments that appear below photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-comment-post-openapi.md
- name: Meetup - Photo Comments v2
  x-api-slug: 2photo-comments-get
  description: This method returns comments on meetup photos. To post messages, see
    the corresponding write method
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/2photo-comments-get-openapi.md
- name: Meetup - Event Photos
  x-api-slug: urlnameeventsevent-idphotos-get
  description: Lists photos for a given event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotos-get-openapi.md
- name: Meetup - Event Photo Upload
  x-api-slug: urlnameeventsevent-idphotos-post
  description: Support for uploading new Event photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotos-post-openapi.md
- name: Meetup - Event Photo
  x-api-slug: urlnameeventsevent-idphotosphoto-id-get
  description: Gets information about a specific photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-get-openapi.md
- name: Meetup - Event Photo Edit
  x-api-slug: urlnameeventsevent-idphotosphoto-id-patch
  description: Edits photo details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-patch-openapi.md
- name: Meetup - Event Photo Delete
  x-api-slug: urlnameeventsevent-idphotosphoto-id-delete
  description: Deletes a specified event photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-id-delete-openapi.md
- name: Meetup - Photo Comment
  x-api-slug: urlnameeventsevent-idphotosphoto-idcomments-post
  description: Creates a new photo comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-post-openapi.md
- name: Meetup - Photo Comments
  x-api-slug: urlnameeventsevent-idphotosphoto-idcomments-get
  description: Lists photo comments associated with a photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-get-openapi.md
- name: Meetup - Photo Comment Delete
  x-api-slug: urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete
  description: Deletes photo comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete-openapi.md
- name: Meetup - Album Photos
  x-api-slug: urlnamephotos-get
  description: Lists of all photos uploaded for the group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephotos-get-openapi.md
- name: Meetup - Photo Album List
  x-api-slug: urlnamephoto-albums-get
  description: Gets a list a group photo albums in ascending order based on the time
    they were created
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albums-get-openapi.md
- name: Meetup - Photo Album
  x-api-slug: urlnamephoto-albumsalbum-id-get
  description: Gets information about a specific photo album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-id-get-openapi.md
- name: Meetup - Album Photos
  x-api-slug: urlnamephoto-albumsalbum-idphotos-get
  description: Lists photos for a given photo album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-idphotos-get-openapi.md
- name: Meetup - Album Photo Upload
  x-api-slug: urlnamephoto-albumsalbum-idphotos-post
  description: Support for uploading new Album photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Meetups, Events, My API Stack, Stack Network, Stack, Media, Marketplace, internet,
    API Provider, API Service Provider, Profiles, General Data, Relative Data, Service
    API, Pedestal, Historical Data API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/photos/master/_listings/meetup/urlnamephoto-albumsalbum-idphotos-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://medium.api.gallery.streamdata.io
- type: x-api-stack
  url: http://meetup.stack.network
- type: x-base
  url: http://api.meetup.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/meetup
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-email
  url: privacy@meetup.com
- type: x-email
  url: abuse@meetup.com
- type: x-email
  url: api_license@meetup.com
- type: x-email
  url: arbitration-opt-out@meetup.com
- type: x-email
  url: legal@meetup.com
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-twitter
  url: https://twitter.com/Meetup
- type: x-website
  url: http://meetup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---