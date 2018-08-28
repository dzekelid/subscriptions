---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Get Subscriptions
  description: Returns subscription resources that match the API request criteria.
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
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---