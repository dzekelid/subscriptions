---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions:
    delete:
      summary: Delete Subscriptions
      description: Deletes a subscription.
      operationId: deleteSubscriptions
      x-api-path-slug: subscriptions-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube subscription ID for the
          resource that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    get:
      summary: Get Subscriptions
      description: Returns subscription resources that match the API request criteria.
      operationId: getSubscriptions
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a YouTube channel ID
      - in: query
        name: forChannelId
        description: The forChannelId parameter specifies a comma-separated list of
          channel IDs
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          subscription ID(s) for the resource(s) that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users subscriptions
      - in: query
        name: myRecentSubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in reverse chronological order (newest first)
      - in: query
        name: mySubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in no particular order
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: order
        description: The order parameter specifies the method that will be used to
          sort resources in the API response
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more subscription resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    post:
      summary: Add Subscriptions
      description: Adds a subscription for the authenticated user's channel.
      operationId: postSubscriptions
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
---