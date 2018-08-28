swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{application}/subscriptions:
    get:
      summary: Get Application Subscriptions
      description: All of the subscriptions this application has for real-time notifications.
      operationId: getApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-get
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions
    post:
      summary: Post Application Subscriptions
      description: Adds a real-time notification subscription for this application.
      operationId: postApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-post
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: callback_url
        description: A callback URL to which Facebook will post subscription updates
      - in: query
        name: fields
        description: List of properties for the `object` to monitor
      - in: query
        name: object
        description: Object to monitor - `user`, `permissions`, or `page`
      - in: query
        name: verify_token
        description: Token sent in the verification request
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions
    delete:
      summary: Delete Application Subscriptions
      description: Deletes a real-time notification subscription for this application.
      operationId: deleteApplicationSubscriptions
      x-api-path-slug: applicationsubscriptions-delete
      parameters:
      - in: path
        name: application
        description: Represents the ID of the application object
      - in: query
        name: object
        description: Object to monitor - `user`, `permissions`, or `page`
      responses:
        200:
          description: OK
      tags:
      - Application
      - Subscriptions