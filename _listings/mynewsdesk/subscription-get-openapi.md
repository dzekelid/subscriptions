---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 0
info:
  title: My News Desk Pressroom List News Subscription
  description: News Subscription
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  subscription/:
    get:
      summary: News Subscription
      description: News Subscription
      operationId: getSubscription
      x-api-path-slug: subscription-get
      parameters:
      - in: query
        name: newsdesk_pressroom
        description: Set the pressroom to search in
      - in: query
        name: newsdesk_subscriber_email
        description: Email address of the subscriber
      - in: query
        name: newsdesk_subscribe_to_type
        description: Send a parameter with the value 1 for each type of material to
          be included in the subscription
      - in: query
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Subscription
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