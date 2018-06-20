---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListEventSubscriptions:
    get:
      summary: List Event Subscriptions
      description: |-
        Lists all the event subscriptions for the assessment template that is specified by
                 the ARN of the assessment template.
      operationId: listEventSubscriptions
      x-api-path-slug: actionlisteventsubscriptions-get
      parameters:
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items you want in the         response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      - in: query
        name: resourceArn
        description: The ARN of the assessment template for which you want to list
          the existing event         subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=SubscribeToEvent:
    get:
      summary: Subscribe To Event
      description: |-
        Enables the process of sending Amazon Simple Notification Service (SNS) notifications
                 about a specified event to a specified SNS topic.
      operationId: subscribeToEvent
      x-api-path-slug: actionsubscribetoevent-get
      parameters:
      - in: query
        name: event
        description: The event for which you want to receive SNS notifications
        type: string
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that is used during the event
          for which you want         to receive SNS notifications
        type: string
      - in: query
        name: topicArn
        description: The ARN of the SNS topic to which the SNS notifications are sent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=UnsubscribeFromEvent:
    get:
      summary: Unsubscribe From Event
      description: |-
        Disables the process of sending Amazon Simple Notification Service (SNS)
                 notifications about a specified event to a specified SNS topic.
      operationId: unsubscribeFromEvent
      x-api-path-slug: actionunsubscribefromevent-get
      parameters:
      - in: query
        name: event
        description: The event for which you want to stop receiving SNS notifications
        type: string
      - in: query
        name: resourceArn
        description: The ARN of the assessment template that is used during the event
          for which you want         to stop receiving SNS notifications
        type: string
      - in: query
        name: topicArn
        description: The ARN of the SNS topic to which SNS notifications are sent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
---