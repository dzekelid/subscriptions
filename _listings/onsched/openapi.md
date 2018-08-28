swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
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
  /consumer/v1/customers/subscriptions/{id}:
    get:
      summary: Returns a customer subscription object.
      description: The result returned is a single customer subscription object.
      operationId: ConsumerV1CustomersSubscriptionsByIdGet
      x-api-path-slug: consumerv1customerssubscriptionsid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer subscription object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    put:
      summary: Updates a customer subscription object.
      description: Use this endpoint to update customer subscription information.
      operationId: ConsumerV1CustomersSubscriptionsByIdPut
      x-api-path-slug: consumerv1customerssubscriptionsid-put
      parameters:
      - in: body
        name: customerSubscriptionUM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the customer subscription object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    delete:
      summary: Deletes a list of lead questions
      description: Deletes a list of lead questions
      operationId: ConsumerV1CustomersSubscriptionsByIdDelete
      x-api-path-slug: consumerv1customerssubscriptionsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions