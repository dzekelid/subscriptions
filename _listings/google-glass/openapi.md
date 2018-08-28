swagger: "2.0"
x-collection-name: Google Glass
x-complete: 1
info:
  title: Google Mirror
  description: interacts-with-glass-users-via-the-timeline-
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