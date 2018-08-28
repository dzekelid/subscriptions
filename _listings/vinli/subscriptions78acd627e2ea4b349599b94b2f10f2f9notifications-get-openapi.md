---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli Get Notifications for a Subscription
  description: Get notifications for a subscription.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/subscriptions:
    post:
      summary: Update a Subscription
      description: Update a subscription.
      operationId: Devices62976d30B6dc40f18422Ccc367572101SubscriptionsPost2
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101subscriptions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get all Subscriptions for a Device
      description: Get all subscriptions for a device.
      operationId: Devices62976d30B6dc40f18422Ccc367572101SubscriptionsGet
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101subscriptions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Subscriptionsa
      - Device
  /subscriptions/4ffd7abb-6c04-45e9-a09a-a669abf4f885:
    get:
      summary: Get a Specific Subscription
      description: Get a specific subscription.
      operationId: Subscriptions4ffd7abb6c0445e9A09aA669abf4f885Get
      x-api-path-slug: subscriptions4ffd7abb6c0445e9a09aa669abf4f885-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Subscription
  /subscriptions/78acd627-e2ea-4b34-9599-b94b2f10f2f9/notifications:
    get:
      summary: Get Notifications for a Subscription
      description: Get notifications for a subscription.
      operationId: Subscriptions78acd627E2ea4b349599B94b2f10f2f9NotificationsGet
      x-api-path-slug: subscriptions78acd627e2ea4b349599b94b2f10f2f9notifications-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Notificationsa
      - Subscription
  /subscriptions/5b6a6164-aa14-4e00-9f50-b5c61faeb167:
    delete:
      summary: Delete a Subscription
      description: Delete a subscription.
      operationId: Subscriptions5b6a6164Aa144e009f50B5c61faeb167Delete
      x-api-path-slug: subscriptions5b6a6164aa144e009f50b5c61faeb167-delete
      parameters:
      - in: header
        name: ac
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
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