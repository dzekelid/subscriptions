---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Update Subscription
  description: Update subscription Renew a subscription by extending its expiry time.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscribedSkus/{id}:
    get:
      summary: Get Subscribed Sku
      description: Get subscribedSku Retrieve a specific commercial subscription that
        an organization has acquired.
      operationId: GetSubscribedSku
      x-api-path-slug: subscribedskusid-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer token
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscribed
      - Sku
  /subscribedSkus:
    get:
      summary: List Subscribed Skus
      description: List subscribedSkus Retrieve the list of commercial subscriptions
        that an organization has acquired.
      operationId: ListSubscribedSkus
      x-api-path-slug: subscribedskus-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer token
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Subscribed
      - Skus
  /groups/{id}/subscribeByMail:
    post:
      summary: Group Subscribe By Mail
      description: 'group: subscribeByMail Calling this method will enable the current
        user to receive email notifications for this group, about new posts, events,
        and files in that group. Supported for only Office 365 groups.'
      operationId: Group:SubscribeByMail
      x-api-path-slug: groupsidsubscribebymail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - SubscribeMail
  /subscriptions/{subscriptionId}:
    delete:
      summary: Delete Subscription
      description: Delete subscription Delete a subscription.
      operationId: DeleteSubscription
      x-api-path-slug: subscriptionssubscriptionid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: subscriptionId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get Subscription
      description: Get subscription Retrieve the properties and relationships of a
        subscription.
      operationId: GetSubscription
      x-api-path-slug: subscriptionssubscriptionid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: subscriptionId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscription
    patch:
      summary: Update Subscription
      description: Update subscription Renew a subscription by extending its expiry
        time.
      operationId: UpdateSubscription
      x-api-path-slug: subscriptionssubscriptionid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: subscriptionId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /subscriptions:
    post:
      summary: Create Subscription
      description: Create subscription Subscribes a listener application to receive
        notifications when data on the Microsoft Graph changes.
      operationId: CreateSubscription
      x-api-path-slug: subscriptions-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
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