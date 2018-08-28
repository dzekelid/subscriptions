---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Post Account Subscriptions
  description: 'Add a new subscription to an account. JSON with subscription details
    is sent. Roles: account/owner, system/admin.'
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/subscriptions:
    post:
      summary: Post Account Subscriptions
      description: 'Add a new subscription to an account. JSON with subscription details
        is sent. Roles: account/owner, system/admin.'
      operationId: addSubscription
      x-api-path-slug: accountsubscriptions-post
      parameters:
      - in: body
        name: body
        description: Subscription details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
  /account/subscriptions/{subscriptionId}:
    delete:
      summary: Delete Account Subscriptions Subscriptionid
      description: 'Remove subscription from account. Roles: account/owner, system/admin.'
      operationId: removeSubscription
      x-api-path-slug: accountsubscriptionssubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
    get:
      summary: Get Account Subscriptions Subscriptionid
      description: Get information on a particular subscription by its unique ID.
      operationId: getSubscriptionById
      x-api-path-slug: accountsubscriptionssubscriptionid-get
      parameters:
      - in: path
        name: subscriptionId
        description: Subscription ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - Subscriptions
      - SubscriptionId
  /account/{accountId}/subscriptions:
    get:
      summary: Get Account Accountid Subscriptions
      description: Get information on account subscriptions. This API call requires
        account/owner, account/member, system/admin or system/manager role.
      operationId: getSubscriptions
      x-api-path-slug: accountaccountidsubscriptions-get
      parameters:
      - in: path
        name: accountId
        description: Account ID
      - in: query
        name: service
        description: Service ID
      responses:
        200:
          description: OK
      tags:
      - Account
      - AccountId
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