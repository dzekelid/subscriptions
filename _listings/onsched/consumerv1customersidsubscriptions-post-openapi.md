---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Creates a new customer subscription object.
  description: Use this endpoint to create a new customer subscription.
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/customers/subscriptions:
    get:
      summary: Returns a list of customer subscriptions.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersSubscriptionsGet
      x-api-path-slug: consumerv1customerssubscriptions-get
      parameters:
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
  /consumer/v1/customers/{id}/subscriptions:
    get:
      summary: Returns a customer subscription object.
      description: The result returned is a single customer subscription object. A
        customer can only be subsribed to a single Customer Plan
      operationId: ConsumerV1CustomersByIdSubscriptionsGet
      x-api-path-slug: consumerv1customersidsubscriptions-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    post:
      summary: Creates a new customer subscription object.
      description: Use this endpoint to create a new customer subscription.
      operationId: ConsumerV1CustomersByIdSubscriptionsPost
      x-api-path-slug: consumerv1customersidsubscriptions-post
      parameters:
      - in: body
        name: customerSubscriptionIM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
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