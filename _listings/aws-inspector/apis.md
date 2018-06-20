---
name: AWS Inspector
x-slug: aws-inspector
description: Amazon Inspector is an automated security assessment service that helps
  improve the security and compliance of applications deployed on AWS. Amazon Inspector
  automatically assesses applications for vulnerabilities or deviations from best
  practices. After performing an assessment, Amazon Inspector produces a detailed
  list of security findings prioritized by level of severity.To help you get started
  quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped
  to common security best practices and vulnerability definitions. Examples of built-in
  rules include checking for remote root login being enabled, or vulnerable software
  versions installed. These rules are regularly updated by AWS security researchers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Subscriptions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Inspector API List Event Subscriptions
  x-api-slug: aws-inspector-api
  description: |-
    Lists all the event subscriptions for the assessment template that is specified by
             the ARN of the assessment template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: ://///?Action=ListEventSubscriptions
  tags: 'Event Subscriptions '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionlisteventsubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionlisteventsubscriptions-get-openapi.md
- name: AWS Inspector API Subscribe To Event
  x-api-slug: aws-inspector-api
  description: |-
    Enables the process of sending Amazon Simple Notification Service (SNS) notifications
             about a specified event to a specified SNS topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: ://///?Action=SubscribeToEvent
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionsubscribetoevent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionsubscribetoevent-get-openapi.md
- name: AWS Inspector API Unsubscribe From Event
  x-api-slug: aws-inspector-api
  description: |-
    Disables the process of sending Amazon Simple Notification Service (SNS)
             notifications about a specified event to a specified SNS topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: ://///?Action=UnsubscribeFromEvent
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionunsubscribefromevent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/actionunsubscribefromevent-get-openapi.md
- name: AWS Inspector API
  x-api-slug: aws-inspector-api
  description: Amazon Inspector is an automated security assessment service that helps
    improve the security and compliance of applications deployed on AWS. Amazon Inspector
    automatically assesses applications for vulnerabilities or deviations from best
    practices. After performing an assessment, Amazon Inspector produces a detailed
    list of security findings prioritized by level of severity.To help you get started
    quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped
    to common security best practices and vulnerability definitions. Examples of built-in
    rules include checking for remote root login being enabled, or vulnerable software
    versions installed. These rules are regularly updated by AWS security researchers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: :///
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-inspector/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/inspector/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/inspector/faqs/
- type: x-getting-started
  url: https://docs.aws.amazon.com/inspector/latest/userguide/inspector_quickstart.html
- type: x-partners
  url: https://aws.amazon.com/inspector/partners/
- type: x-pricing
  url: https://aws.amazon.com/inspector/pricing/
- type: x-testimonials
  url: https://aws.amazon.com/inspector/customers/
- type: x-website
  url: https://aws.amazon.com/inspector/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---