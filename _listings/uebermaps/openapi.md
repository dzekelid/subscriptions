swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions:
    get:
      summary: List subscriptions. Pass no parameters to get own subscriptions
      description: List subscriptions.
      operationId: subscriptions.get
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: map_id
        description: Id of map
      - in: query
        name: user_id
        description: Id of user
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Subscriptions
      - ""
      - Pass
      - "No"
      - Parameters
      - To
      - Get
      - Own
      - Subscriptions
    post:
      summary: Create map subscription
      description: Create map subscription.
      operationId: subscriptions.post
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: map_id
        description: map id
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Map
      - Subscription
  /maps/{id}/subscriptions:
    get:
      summary: List subscriptions for a given map
      description: List subscriptions for a given map.
      operationId: maps.id.subscriptions.get
      x-api-path-slug: mapsidsubscriptions-get
      parameters:
      - in: path
        name: id
        description: Id of map
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Subscriptionsa
      - Given
      - Map