---
swagger: "2.0"
info:
  title: Instagram
  description: 'The first version of the Instagram API is an exciting step forward
    towardsmaking it easier for users to have open access to their data. We created
    itso that you can surface the amazing content Instagram users share everysecond,
    in fun and innovative ways.Build something great!Once you''ve[registered your
    client](http://instagram.com/developer/register/) it''s easyto start requesting
    data from Instagram.All endpoints are only accessible via https and are located
    at`api.instagram.com`. For instance: you can grab the most popular photos atthe
    moment by accessing the following URL with your client ID(replace CLIENT-ID with
    your own):```  https://api.instagram.com/v1/media/popular?client_id=CLIENT-ID```You''re
    best off using an access_token for the authenticated user for eachendpoint, though
    many endpoints don''t require it.In some cases an access_token will give you more
    access to information, andin all cases, it means that you are operating under
    a per-access_token limitvs. the same limit for your single client_id.## LimitsBe
    nice. If you''re sending too many requests too quickly, we''ll send back a`503`
    error code (server unavailable).You are limited to 5000 requests per hour per
    `access_token` or `client_id`overall. Practically, this means you should (when
    possible) authenticateusers so that limits are well outside the reach of a given
    user.## Deleting ObjectsWe do our best to have all our URLs be[RESTful](http://en.wikipedia.org/wiki/Representational_state_transfer).Every
    endpoint (URL) may support one of four different http verbs. GETrequests fetch
    information about an object, POST requests create objects,PUT requests update
    objects, and finally DELETE requests will deleteobjects.Since many old browsers
    don''t support PUT or DELETE, we''ve made it easy tofake PUTs and DELETEs. All
    you have to do is do a POST with _method=PUT or_method=DELETE as a parameter and
    we will treat it as if you used PUT orDELETE respectively.## Structure### The
    EnvelopeEvery response is contained by an envelope. That is, each response has
    apredictable set of keys with which you can expect to interact:```json{    &quot;meta&quot;:
    {        &quot;code&quot;: 200    },    &quot;data&quot;: {        ...    },    &quot;pagination&quot;:
    {        &quot;next_url&quot;: &quot;...&quot;,        &quot;next_max_id&quot;:
    &quot;13872296&quot;    }}```#### METAThe meta key is used to communicate extra
    information about the response tothe developer. If all goes well, you''ll only
    ever see a code key with value200. However, sometimes things go wrong, and in
    that case you might see aresponse like:```json{    &quot;meta&quot;: {        &quot;error_type&quot;:
    &quot;OAuthException&quot;,        &quot;code&quot;: 400,        &quot;error_message&quot;:
    &quot;...&quot;    }}```#### DATAThe data key is the meat of the response. It
    may be a list or dictionary,but either way this is where you''ll find the data
    you requested.#### PAGINATIONSometimes you just can''t get enough. For this reason,
    we''ve provided aconvenient way to access more data in any request for sequential
    data.Simply call the url in the next_url parameter and we''ll respond with thenext
    set of data.```json{    ...    &quot;pagination&quot;: {        &quot;next_url&quot;:
    &quot;https://api.instagram.com/v1/tags/puppy/media/recent?access_token=fb2e77d.47a0479900504cb3ab4a1f626d174d2d&amp;max_id=13872296&quot;,        &quot;next_max_id&quot;:
    &quot;13872296&quot;    }}```On views where pagination is present, we also support
    the &quot;count&quot; parameter.Simply set this to the number of items you''d
    like to receive. Note that thedefault values should be fine for most applications
    - but if you decide toincrease this number there is a maximum value defined on
    each endpoint.### JSONPIf you''re writing an AJAX application, and you''d like
    to wrap our responsewith a callback, all you have to do is specify a callback
    parameter withany API call:```https://api.instagram.com/v1/tags/coffee/media/recent?access_token=fb2e77d.47a0479900504cb3ab4a1f626d174d2d&amp;callback=callbackFunction```Would
    respond with:```jscallbackFunction({    ...});```'
  version: v1
host: api.instagram.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/{media-id}/comments:
    get:
      summary: MediaCommentsByMediaId
      description: Get a list of recent comments on a media object
      operationId: MediaCommentsByMediaIdGet
      parameters:
      - in: path
        name: media-id
        description: Media ID
      responses:
        200:
          description: OK
      tags:
      - photos
      - comments
definitions:
  User:
    properties:
      id:
        description: This is a default description.
        type: get
      username:
        description: This is a default description.
        type: get
      full_name:
        description: This is a default description.
        type: get
      profile_picture:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
      website:
        description: This is a default description.
        type: get
  Counts:
    properties:
      media:
        description: This is a default description.
        type: get
      follows:
        description: This is a default description.
        type: get
      follwed_by:
        description: This is a default description.
        type: get
  Media:
    properties:
      created_time:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      filter:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      users_in_photo:
        description: This is a default description.
        type: get
  Tag:
    properties:
      media_count:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  MiniProfile:
    properties:
      user_name:
        description: This is a default description.
        type: get
      full_name:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      profile_picture:
        description: This is a default description.
        type: get
  Location:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  Comments:
    properties:
      count:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
  Comment:
    properties:
      id:
        description: This is a default description.
        type: get
      created_time:
        description: This is a default description.
        type: get
      text:
        description: This is a default description.
        type: get
  Likes:
    properties:
      count:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
  Images:
    properties: []
  Image:
    properties:
      width:
        description: This is a default description.
        type: get
      height:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  Videos:
    properties: []
  Like:
    properties:
      user_name:
        description: This is a default description.
        type: get
      first_name:
        description: This is a default description.
        type: get
      last_name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
  UsersByUserIdResponse:
    properties: []
  UsersSelfFeedResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersMediaRecentByUserIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersSelfMediaLikedResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersSearchResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersFollowsByUserIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersFollowedByByUserIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  UsersSelfRequestedByResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  Meta:
    properties:
      code:
        description: This is a default description.
        type: get
  UsersRelationshipByUserIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  MediaSearchResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  Datum:
    properties:
      created_time:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      filter:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      users_in_photo:
        description: This is a default description.
        type: get
      distance:
        description: This is a default description.
        type: get
  MediaPopularResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  MediaCommentsByMediaIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  Meta32:
    properties:
      code:
        description: This is a default description.
        type: get
  MediaCommentsByMediaIdResponse33:
    properties:
      data:
        description: This is a default description.
        type: get
  MediaLikesByMediaIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  MediaLikesByMediaIdResponse39:
    properties:
      data:
        description: This is a default description.
        type: get
  TagsMediaRecentByTagNameResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  TagsSearchResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  LocationsByLocationIdResponse:
    properties: []
  LocationsMediaRecentByLocationIdResponse:
    properties:
      data:
        description: This is a default description.
        type: get
  LocationsSearchResponse:
    properties:
      data:
        description: This is a default description.
        type: get
x-collection-name: Instagram
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