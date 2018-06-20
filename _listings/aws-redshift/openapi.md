---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateEventSubscription:
    get:
      summary: Create Event Subscription
      description: Creates an Amazon Redshift event notification subscription.
      operationId: createEventSubscription
      x-api-path-slug: actioncreateeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription, set
          to                false to create the subscription but not active it
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: Specifies the Amazon Redshift event categories to be published
          by the event notification            subscription
        type: string
      - in: query
        name: Severity
        description: Specifies the Amazon Redshift event severity to be published
          by the event notification            subscription
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic used to
          transmit the event            notifications
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: A list of one or more identifiers of Amazon Redshift source objects
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the event subscription to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DeleteEventSubscription:
    get:
      summary: Delete Event Subscription
      description: Deletes an Amazon Redshift event notification subscription.
      operationId: deleteEventSubscription
      x-api-path-slug: actiondeleteeventsubscription-get
      parameters:
      - in: query
        name: SubscriptionName
        description: The name of the Amazon Redshift event notification subscription
          to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DescribeEventSubscriptions:
    get:
      summary: Describe Event Subscriptions
      description: |-
        Lists descriptions of all the Amazon Redshift event notifications subscription for a
                    customer account.
      operationId: describeEventSubscriptions
      x-api-path-slug: actiondescribeeventsubscriptions-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the Amazon Redshift event notification subscription
          to be            described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=ModifyEventSubscription:
    get:
      summary: Modify Event Subscription
      description: Modifies an existing Amazon Redshift event notification subscription.
      operationId: modifyEventSubscription
      x-api-path-slug: actionmodifyeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value indicating if the subscription is enabled
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: Specifies the Amazon Redshift event categories to be published
          by the event notification            subscription
        type: string
      - in: query
        name: Severity
        description: Specifies the Amazon Redshift event severity to be published
          by the event notification            subscription
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic to be used by
          the event            notification subscription
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: A list of one or more identifiers of Amazon Redshift source objects
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the modified Amazon Redshift event notification subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
---