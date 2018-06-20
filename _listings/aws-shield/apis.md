---
name: AWS Shield
x-slug: aws-shield
description: AWS Shield is a managed Distributed Denial of Service protection service
  that safeguards web applications running on AWS. AWS Shield provides always-on detection
  and automatic inline mitigations that minimize application downtime and latency,
  so there is no need to engage AWS Support to benefit from DDoS protection. There
  are two tiers of AWS Shield, Standard and Advanced. All AWS customers benefit from
  the automatic protections of AWS Shield Standard, at no additional charge. AWS Shield
  Standard defends against most common, frequently occurring network and transport
  layer DDoS attacks that target your web site or applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2016-12-30 at 10.35.48 PM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Subscriptions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-shield/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Shield API Describe Subscription
  x-api-slug: aws-shield-api
  description: Provides details about the AWS Shield Advanced subscription for an
    account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-12-30 at 10.35.48 PM.png
  humanURL: https://aws.amazon.com/shield/
  baseURL: ://///?Action=DescribeSubscription
  tags: Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-shield/actiondescribesubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-shield/actiondescribesubscription-get-openapi.md
- name: AWS Shield API
  x-api-slug: aws-shield-api
  description: AWS Shield is a managed Distributed Denial of Service protection service
    that safeguards web applications running on AWS. AWS Shield provides always-on
    detection and automatic inline mitigations that minimize application downtime
    and latency, so there is no need to engage AWS Support to benefit from DDoS protection.
    There are two tiers of AWS Shield, Standard and Advanced. All AWS customers benefit
    from the automatic protections of AWS Shield Standard, at no additional charge.
    AWS Shield Standard defends against most common, frequently occurring network
    and transport layer DDoS attacks that target your web site or applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2016-12-30 at 10.35.48 PM.png
  humanURL: https://aws.amazon.com/shield/
  baseURL: :///
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/aws-shield/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/waf/latest/APIReference/
- type: x-documentation
  url: http://docs.aws.amazon.com/waf/latest/DDOSAPIReference/Welcome.htm
- type: x-faq
  url: https://aws.amazon.com/shield/faqs/
- type: x-pricing
  url: https://aws.amazon.com/shield/pricing/
- type: x-website
  url: https://aws.amazon.com/shield/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---