---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API List Event Subscriptions
  version: 1.0.0
  description: |-
    Lists all the event subscriptions for the assessment template that is specified by
             the ARN of the assessment template.
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