---
swagger: "2.0"
x-collection-name: Google Glass
x-complete: 0
info:
  title: Google Glass APIs Delete Subscription
  description: Deletes a subscription.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /mirror/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions:
    get:
      summary: Get Subscriptions
      description: Retrieves a list of subscriptions for the authenticated user and
        service.
      operationId: mirror.subscriptions.list
      x-api-path-slug: subscriptions-get
      responses:
        200:
          description: OK
      tags:
      - Subscription
    post:
      summary: Create Subscription
      description: Creates a new subscription.
      operationId: mirror.subscriptions.insert
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /subscriptions/{id}:
    delete:
      summary: Delete Subscription
      description: Deletes a subscription.
      operationId: mirror.subscriptions.delete
      x-api-path-slug: subscriptionsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the subscription
      responses:
        200:
          description: OK
      tags:
      - Subscription
    put:
      summary: Update Subscription
      description: Updates an existing subscription in place.
      operationId: mirror.subscriptions.update
      x-api-path-slug: subscriptionsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the subscription
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