---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API List Subscriptions
  version: 1.0.0
  description: Returns a list of the requester's subscriptions.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ConfirmSubscription:
    get:
      summary: Confirm Subscription
      description: |-
        Verifies an endpoint owner's intent to receive messages by validating the token sent to the
              endpoint by an earlier Subscribe action.
      operationId: confirmSubscription
      x-api-path-slug: actionconfirmsubscription-get
      parameters:
      - in: query
        name: AuthenticateOnUnsubscribe
        description: Disallows unauthenticated unsubscribes of the subscription
        type: string
      - in: query
        name: Token
        description: Short-lived token sent to an endpoint during the Subscribe action
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to confirm a subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=GetSubscriptionAttributes:
    get:
      summary: Get Subscription Attributes
      description: Returns all of the properties of a subscription.
      operationId: getSubscriptionAttributes
      x-api-path-slug: actiongetsubscriptionattributes-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListSubscriptions:
    get:
      summary: List Subscriptions
      description: Returns a list of the requester's subscriptions.
      operationId: listSubscriptions
      x-api-path-slug: actionlistsubscriptions-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListSubscriptionsByTopic:
    get:
      summary: List Subscriptions By Topic
      description: Returns a list of the subscriptions to a specific topic.
      operationId: listSubscriptionsByTopic
      x-api-path-slug: actionlistsubscriptionsbytopic-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptionsByTopic request
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to find subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=SetSubscriptionAttributes:
    get:
      summary: Set Subscription Attributes
      description: Allows a subscription owner to set an attribute of the topic to
        a new value.
      operationId: setSubscriptionAttributes
      x-api-path-slug: actionsetsubscriptionattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute in JSON format
        type: string
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=Subscribe:
    get:
      summary: Subscribe
      description: Prepares to subscribe an endpoint by sending the endpoint a confirmation
        message.
      operationId: subscribe
      x-api-path-slug: actionsubscribe-get
      parameters:
      - in: query
        name: Endpoint
        description: The endpoint that you want to receive notifications
        type: string
      - in: query
        name: Protocol
        description: The protocol you want to use
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to subscribe to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
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