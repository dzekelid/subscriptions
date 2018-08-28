swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 1
info:
  title: Google Cloud Pub/Sub
  description: provides-reliable-manytomany-asynchronous-messaging-between-applications-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: pubsub.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{project}/subscriptions:
    get:
      summary: List Matching Subscription
      description: Lists matching subscriptions.
      operationId: pubsub.projects.subscriptions.list
      x-api-path-slug: v1projectsubscriptions-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of subscriptions to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListSubscriptionsResponse`; indicates
          thatthis is a continuation of a prior `ListSubscriptions` call, and that
          thesystem should return the next page of data
      - in: path
        name: project
        description: The name of the cloud project that subscriptions belong to
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:
    delete:
      summary: Delete Subscription
      description: |-
        Deletes an existing subscription. All messages retained in the subscription
        are immediately dropped. Calls to `Pull` after deletion will return
        `NOT_FOUND`. After a subscription is deleted, a new one may be created with
        the same name, but the new one has no association with the old
        subscription or its topic unless the same topic is specified.
      operationId: pubsub.projects.subscriptions.delete
      x-api-path-slug: v1subscription-delete
      parameters:
      - in: path
        name: subscription
        description: The subscription to delete
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get Subscription
      description: Gets the configuration details of a subscription.
      operationId: pubsub.projects.subscriptions.get
      x-api-path-slug: v1subscription-get
      parameters:
      - in: path
        name: subscription
        description: The name of the subscription to get
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:acknowledge:
    post:
      summary: Acknowledge Subscription
      description: |-
        Acknowledges the messages associated with the `ack_ids` in the
        `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
        from the subscription.

        Acknowledging a message whose ack deadline has expired may succeed,
        but such a message may be redelivered later. Acknowledging a message more
        than once will not result in an error.
      operationId: pubsub.projects.subscriptions.acknowledge
      x-api-path-slug: v1subscriptionacknowledge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The subscription whose message is being acknowledged
      responses:
        200:
          description: OK
      tags:
      - Subscription