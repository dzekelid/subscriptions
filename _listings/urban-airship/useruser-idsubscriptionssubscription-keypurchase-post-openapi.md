---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Post User User Subscriptions Subscription Key Purchase
  description: Adds a new subscription.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/available_subscriptions:
    get:
      summary: Get User User Available Subscriptions
      description: Retrieves subscription options.
      operationId: user.user_id.available_subscriptions.get
      x-api-path-slug: useruser-idavailable-subscriptions-get
      parameters:
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Available
      - Subscriptions
  /user/{user_id}/subscriptions/{subscription_key}/purchase:
    post:
      summary: Post User User Subscriptions Subscription Key Purchase
      description: Adds a new subscription.
      operationId: user.user_id.subscriptions.subscription_key.purchase.post
      x-api-path-slug: useruser-idsubscriptionssubscription-keypurchase-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: subscription_key
        description: Subscription Key
      - in: path
        name: subscription_key
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscriptions
      - Subscription
      - Key
      - Purchase
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