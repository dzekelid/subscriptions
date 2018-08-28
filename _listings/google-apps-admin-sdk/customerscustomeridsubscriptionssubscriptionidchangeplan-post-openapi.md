---
swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 0
info:
  title: Google Apps Admin SDK API Update Subscription
  version: 1.0.0
  description: Update a subscription plan. Use this method to update a plan for a
    30-day trial or a flexible plan subscription to an annual commitment plan with
    monthly or yearly payments.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{customerId}/subscriptions:
    post:
      summary: Create Subscription
      description: Create or transfer a subscription.
      operationId: reseller.subscriptions.insert
      x-api-path-slug: customerscustomeridsubscriptions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: customerAuthToken
        description: The customerAuthToken query string is required when creating
          a resold account that transfers a direct customers subscription or transfers
          another reseller customers subscription to your reseller management
      - in: path
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /customers/{customerId}/subscriptions/{subscriptionId}:
    delete:
      summary: Cancel Subscription
      description: Cancel, suspend or transfer a subscription to direct.
      operationId: reseller.subscriptions.delete
      x-api-path-slug: customerscustomeridsubscriptionssubscriptionid-delete
      parameters:
      - in: path
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      - in: query
        name: deletionType
        description: The deletionType query string enables the cancellation, downgrade,
          or suspension of a subscription
      - in: path
        name: subscriptionId
        description: This is a required property
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get Subscription
      description: Get a specific subscription.
      operationId: reseller.subscriptions.get
      x-api-path-slug: customerscustomeridsubscriptionssubscriptionid-get
      parameters:
      - in: path
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      - in: path
        name: subscriptionId
        description: This is a required property
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /customers/{customerId}/subscriptions/{subscriptionId}/activate:
    post:
      summary: Activate Subscription
      description: Activates a subscription previously suspended by the reseller
      operationId: reseller.subscriptions.activate
      x-api-path-slug: customerscustomeridsubscriptionssubscriptionidactivate-post
      parameters:
      - in: path
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      - in: path
        name: subscriptionId
        description: This is a required property
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /customers/{customerId}/subscriptions/{subscriptionId}/changePlan:
    post:
      summary: Update Subscription
      description: Update a subscription plan. Use this method to update a plan for
        a 30-day trial or a flexible plan subscription to an annual commitment plan
        with monthly or yearly payments.
      operationId: reseller.subscriptions.changePlan
      x-api-path-slug: customerscustomeridsubscriptionssubscriptionidchangeplan-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      - in: path
        name: subscriptionId
        description: This is a required property
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /subscriptions:
    get:
      summary: List Subscriptions
      description: List of subscriptions managed by the reseller. The list can be
        all subscriptions, all of a customer's subscriptions, or all of a customer's
        transferable subscriptions.
      operationId: reseller.subscriptions.list
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: customerAuthToken
        description: The customerAuthToken query string is required when creating
          a resold account that transfers a direct customers subscription or transfers
          another reseller customers subscription to your reseller management
      - in: query
        name: customerId
        description: Either the customers primary domain name or the customers unique
          identifier
      - in: query
        name: customerNamePrefix
        description: When retrieving all of your subscriptions and filtering for specific
          customers, you can enter a prefix for a customer name
      - in: query
        name: maxResults
        description: When retrieving a large list, the maxResults is the maximum number
          of results per page
      - in: query
        name: pageToken
        description: Token to specify next page in the list
      responses:
        200:
          description: OK
      tags:
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