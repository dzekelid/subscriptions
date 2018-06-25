---
name: AWS Simple Notification Service
x-slug: aws-simple-notification-service
description: Amazon Simple Notification Service (Amazon SNS) is a fast, flexible,
  fully managed push notification service that lets you send individual messages or
  to fan-out messages to large numbers of recipients. Amazon SNS makes it simple and
  cost effective to send push notifications to mobile device users, email recipients
  or even send messages to other distributed services.With Amazon SNS, you can send
  notifications to Apple, Google, Fire OS, and Windows devices, as well as to Android
  devices in China with Baidu Cloud Push. You can use SNS to send SMS messages to
  mobile device users worldwide.Beyond these endpoints, Amazon SNS can also deliver
  messages toAmazon Simple Queue Service(SQS),AWS Lambda functions, or to any HTTP
  endpoint.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Subscriptions
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Notification Service API Confirm Subscription
  x-api-slug: aws-simple-notification-service-api
  description: |-
    Verifies an endpoint owner's intent to receive messages by validating the token sent to the
          endpoint by an earlier Subscribe action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: ://///?Action=ConfirmSubscription
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionconfirmsubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionconfirmsubscription-get-openapi.md
- name: AWS Simple Notification Service API Get Subscription Attributes
  x-api-slug: aws-simple-notification-service-api
  description: Returns all of the properties of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: ://///?Action=GetSubscriptionAttributes
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API List Subscriptions
  x-api-slug: aws-simple-notification-service-api
  description: Returns a list of the requester's subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: ://///?Action=ListSubscriptions
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionlistsubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionlistsubscriptions-get-openapi.md
- name: AWS Simple Notification Service API List Subscriptions By Topic
  x-api-slug: aws-simple-notification-service-api
  description: Returns a list of the subscriptions to a specific topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: ://///?Action=ListSubscriptionsByTopic
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionlistsubscriptionsbytopic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionlistsubscriptionsbytopic-get-openapi.md
- name: AWS Simple Notification Service API Set Subscription Attributes
  x-api-slug: aws-simple-notification-service-api
  description: Allows a subscription owner to set an attribute of the topic to a new
    value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: ://///?Action=SetSubscriptionAttributes
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API
  x-api-slug: aws-simple-notification-service-api
  description: Amazon Simple Notification Service (Amazon SNS) is a fast, flexible,
    fully managed push notification service that lets you send individual messages
    or to fan-out messages to large numbers of recipients. Amazon SNS makes it simple
    and cost effective to send push notifications to mobile device users, email recipients
    or even send messages to other distributed services.With Amazon SNS, you can send
    notifications to Apple, Google, Fire OS, and Windows devices, as well as to Android
    devices in China with Baidu Cloud Push. You can use SNS to send SMS messages to
    mobile device users worldwide.Beyond these endpoints, Amazon SNS can also deliver
    messages toAmazon Simple Queue Service(SQS),AWS Lambda functions, or to any HTTP
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-simple-notification-service/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SN
- type: x-console
  url: https://console.aws.amazon.com/sns
- type: x-documentation
  url: http://docs.aws.amazon.com/sns/latest/api/
- type: x-faq
  url: https://aws.amazon.com/sns/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=72
- type: x-getting-started
  url: https://aws.amazon.com/sns/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/sns/pricing/
- type: x-website
  url: https://aws.amazon.com/sns/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---