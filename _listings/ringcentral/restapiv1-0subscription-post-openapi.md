---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Create Subscription
  description: "Creates a new subscription.\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [deliveryMode.verificationToken] value is invalid\n\n\n400\nSUB-515\nSubscription
    containing only reminder filter is not allowed\n\n\n400\nSUB-522\nWebHook responds
    with incorrect HTTP status. HTTP status is 500\n\n\n400\nSUB-525\nWebHook server
    response is invalid\n\n\n401\nAGW-401\nAuthorization header is not specified\n\n\n401\nAGW-402\nInvalid
    Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n403\nSUB-406\nNot
    allowed subscribe for events to extensions of other account\n\n\n403\nSUB-408\nNot
    allowed subscribe for unknown user\n\n\n403\nSUB-505\nSubscriptions limit exceeded\n\n\n403\nSUB-518\nNot
    allowed subscribe for favorite contacts list changes of another extension\n\n\n403\nSUB-527\nNot
    allowed subscribe for missed calls of another extension\n\n\n403\nSUB-528\n[SubscriptionAPNS]
    application permission is required for [PubNub/APNS] transport\n\n\n403\nSUB-530\nNot
    allowed subscribe for incoming calls of another extension\n\n\n403\nSUB-531\nNot
    allowed subscribe for presence of presence-lines of another extension\n\n\n404\nCMN-102\nResource
    for parameter [dashboardId] is not found"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/subscription:
    get:
      summary: Get Subscriptions
      description: |-
        Returns a list of subscriptions created by a particular user on a particular client app.
        Usage Plan Group
        Light
      operationId: listSubscriptions
      x-api-path-slug: restapiv1-0subscription-get
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    post:
      summary: Create Subscription
      description: "Creates a new subscription.\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [deliveryMode.verificationToken] value is invalid\n\n\n400\nSUB-515\nSubscription
        containing only reminder filter is not allowed\n\n\n400\nSUB-522\nWebHook
        responds with incorrect HTTP status. HTTP status is 500\n\n\n400\nSUB-525\nWebHook
        server response is invalid\n\n\n401\nAGW-401\nAuthorization header is not
        specified\n\n\n401\nAGW-402\nInvalid Authorization header\n\n\n401\nCMN-405\nLogin
        to extension required\n\n\n403\nSUB-406\nNot allowed subscribe for events
        to extensions of other account\n\n\n403\nSUB-408\nNot allowed subscribe for
        unknown user\n\n\n403\nSUB-505\nSubscriptions limit exceeded\n\n\n403\nSUB-518\nNot
        allowed subscribe for favorite contacts list changes of another extension\n\n\n403\nSUB-527\nNot
        allowed subscribe for missed calls of another extension\n\n\n403\nSUB-528\n[SubscriptionAPNS]
        application permission is required for [PubNub/APNS] transport\n\n\n403\nSUB-530\nNot
        allowed subscribe for incoming calls of another extension\n\n\n403\nSUB-531\nNot
        allowed subscribe for presence of presence-lines of another extension\n\n\n404\nCMN-102\nResource
        for parameter [dashboardId] is not found"
      operationId: createSubscription
      x-api-path-slug: restapiv1-0subscription-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /restapi/v1.0/subscription/{subscriptionId}:
    get:
      summary: Get Subscription
      description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
        for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
      operationId: loadSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-get
      parameters:
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Subscription
    put:
      summary: Renew Subscription / Update Event Filters
      description: "Renews the existent subscription if the request body is empty.
        If event filters are specified, calling this method modifies the event filters
        for the existing subscription. The client application can extend or narrow
        the events for which it receives notifications in the frame of one subscription.\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is
        not found"
      operationId: updateSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-put
      parameters:
      - in: query
        name: aggregated
        description: If True then aggregated presence status is returned in a notification
          payload
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Renew
      - Subscription
      - ""
      - ""
      - ""
      - Event
      - Filters
    delete:
      summary: Cancel Subscription
      description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [subscriptionId] is not found"
      operationId: deleteSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription
  /restapi/v1.0/subscription/{subscriptionId}/renew:
    post:
      summary: Renew Subscription
      description: |-
        Renews an existent subscription by ID by posting request with an empty body.
        Usage Plan Group
        Light
      operationId: renewSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionidrenew-post
      parameters:
      - in: path
        name: subscriptionId
      responses:
        200:
          description: OK
      tags:
      - Renew
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