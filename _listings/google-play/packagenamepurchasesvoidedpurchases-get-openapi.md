---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play List Cancelled Purches
  version: 1.0.0
  description: Lists the purchases that were cancelled, refunded or charged-back.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:
    get:
      summary: Check User Subscriptions
      description: Checks whether a user's subscription purchase is valid and returns
        its expiry time.
      operationId: androidpublisher.purchases.subscriptions.get
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstoken-get
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:cancel:
    post:
      summary: Cancel User Subscription
      description: Cancels a user's subscription purchase. The subscription remains
        valid until its expiration time.
      operationId: androidpublisher.purchases.subscriptions.cancel
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokencancel-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:defer:
    post:
      summary: Defer User Subscription
      description: Defers a user's subscription purchase until a specified future
        expiration time.
      operationId: androidpublisher.purchases.subscriptions.defer
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokendefer-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:refund:
    post:
      summary: Refund User Subscription
      description: Refunds a user's subscription purchase, but the subscription remains
        valid until its expiration time and it will continue to recur.
      operationId: androidpublisher.purchases.subscriptions.refund
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokenrefund-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:revoke:
    post:
      summary: Refunds and Revoke
      description: Refunds and immediately revokes a user's subscription purchase.
        Access to the subscription will be terminated immediately and it will stop
        recurring.
      operationId: androidpublisher.purchases.subscriptions.revoke
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokenrevoke-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/voidedpurchases:
    get:
      summary: List Cancelled Purches
      description: Lists the purchases that were cancelled, refunded or charged-back.
      operationId: androidpublisher.purchases.voidedpurchases.list
      x-api-path-slug: packagenamepurchasesvoidedpurchases-get
      parameters:
      - in: query
        name: endTime
        description: The time, in milliseconds since the Epoch, of the newest voided
          in-app product purchase that you want to see in the response
      - in: query
        name: maxResults
      - in: path
        name: packageName
        description: The package name of the application for which voided purchases
          need to be returned (for example, com
      - in: query
        name: startIndex
      - in: query
        name: startTime
        description: The time, in milliseconds since the Epoch, of the oldest voided
          in-app product purchase that you want to see in the response
      - in: query
        name: token
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