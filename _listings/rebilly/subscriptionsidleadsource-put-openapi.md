---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a Lead Source for a Subscription
  description: Create a Lead Source for a Subscription
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions:
    get:
      summary: Retrieve a list of subscriptions
      description: Retrieve a list of subscriptions
      operationId: subscriptions.get
      x-api-path-slug: subscriptions-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Subscriptions
    post:
      summary: Create a subscription
      description: Create a subscription
      operationId: subscriptions.post
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: body
        description: Subscription resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /subscriptions/{id}/lead-source:
    get:
      summary: Retrieve a subscription's Lead Source
      description: Retrieve a Lead Source of given subscription
      operationId: subscriptions.id.lead_source.get
      x-api-path-slug: subscriptionsidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Subscriptions
      - Lead
      - Source
    delete:
      summary: Delete a Lead Source for a Subscription
      description: Delete a Lead Source that belongs to a certain Subscription
      operationId: subscriptions.id.lead_source.delete
      x-api-path-slug: subscriptionsidleadsource-delete
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Subscription
    put:
      summary: Create a Lead Source for a Subscription
      description: Create a Lead Source for a Subscription
      operationId: subscriptions.id.lead_source.put
      x-api-path-slug: subscriptionsidleadsource-put
      parameters:
      - in: body
        name: body
        description: Lead Source resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Subscription
  /subscriptions/{id}:
    get:
      summary: Retrieve a subscription
      description: Retrieve a subscription with specified identifier string
      operationId: subscriptions.id.get
      x-api-path-slug: subscriptionsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Subscription
    put:
      summary: Create or update a subscription with predefined ID
      description: Create or update a subscription with predefined identifier string
      operationId: subscriptions.id.put
      x-api-path-slug: subscriptionsid-put
      parameters:
      - in: body
        name: body
        description: Subscription resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Subscription
      - Predefined
      - ID
  /subscriptions/{id}/cancel:
    post:
      summary: Cancel a subscription
      description: Cancel a subscription
      operationId: subscriptions.id.cancel.post
      x-api-path-slug: subscriptionsidcancel-post
      parameters:
      - in: body
        name: body
        description: Only policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription
  /subscriptions/{id}/matched-rules:
    get:
      summary: Get matched rules for the subscription
      description: Get matched rules for the subscription
      operationId: subscriptions.id.matched_rules.get
      x-api-path-slug: subscriptionsidmatchedrules-get
      responses:
        200:
          description: OK
      tags:
      - Matched
      - Rulesthe
      - Subscription
  /subscriptions/{id}/switch:
    post:
      summary: Switch a subscription
      description: Switch a subscription
      operationId: subscriptions.id.switch.post
      x-api-path-slug: subscriptionsidswitch-post
      parameters:
      - in: body
        name: body
        description: SubscriptionSwitch resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Subscription
  /tracking/subscriptions:
    get:
      summary: Retrieve a list of tracking subscription logs
      description: ""
      operationId: ""
      x-api-path-slug: trackingsubscriptions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tracking
      - Subscription
      - Logs
  /tracking/subscriptions/{id}:
    get:
      summary: Retrieve a tracking subscription log with specified identifier string
      description: ""
      operationId: ""
      x-api-path-slug: trackingsubscriptionsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Tracking
      - Subscription
      - Log
      - Specified
      - Identifier
      - String
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