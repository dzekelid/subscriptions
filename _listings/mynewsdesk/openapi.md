swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 1
info:
  title: My News Desk Pressroom List
  description: mynewsdesk-webservice-for-newsroom-is-a-way-for-you-as-a-registered-customer-to-fetch-information-from-your-newsroom-at-mynewsdesk-to-any-system--you-can-get-all-your-information-as-xml-and-create-email-subscriptions-to-your-material-
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