---
name: Google Cloud Pub Sub
x-slug: google-cloud-pub-sub
description: Cloud Pub/Sub is a fully-managed real-time messaging service that allows
  you to send and receive messages between independent applications. You can leverage
  Cloud Pub/Sub&rsquo;s flexibility to decouple systems and components hosted on Google
  Cloud Platform or elsewhere on the Internet. By building on the same technology
  Google uses, Cloud Pub/Sub is designed to provide &ldquo;at least once&rdquo; delivery
  at low latency with on-demand scalability to 1 million messages per second (and
  beyond).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Subscriptions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Pub/Sub - List Matching Subscription
  x-api-slug: v1projectsubscriptions-get
  description: Lists matching subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1projectsubscriptions-get-openapi.md
- name: Google Cloud Pub/Sub - Delete Subscription
  x-api-slug: v1subscription-delete
  description: |-
    Deletes an existing subscription. All messages retained in the subscription
    are immediately dropped. Calls to `Pull` after deletion will return
    `NOT_FOUND`. After a subscription is deleted, a new one may be created with
    the same name, but the new one has no association with the old
    subscription or its topic unless the same topic is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-delete-openapi.md
- name: Google Cloud Pub/Sub - Get Subscription
  x-api-slug: v1subscription-get
  description: Gets the configuration details of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-get-openapi.md
- name: Google Cloud Pub/Sub - Acknowledge Subscription
  x-api-slug: v1subscriptionacknowledge-post
  description: |-
    Acknowledges the messages associated with the `ack_ids` in the
    `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
    from the subscription.

    Acknowledging a message whose ack deadline has expired may succeed,
    but such a message may be redelivered later. Acknowledging a message more
    than once will not result in an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscriptionacknowledge-post-openapi.md
- name: Google Cloud Pub/Sub - List Matching Subscription
  x-api-slug: v1projectsubscriptions-get
  description: Lists matching subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1projectsubscriptions-get-openapi.md
- name: Google Cloud Pub/Sub - Delete Subscription
  x-api-slug: v1subscription-delete
  description: |-
    Deletes an existing subscription. All messages retained in the subscription
    are immediately dropped. Calls to `Pull` after deletion will return
    `NOT_FOUND`. After a subscription is deleted, a new one may be created with
    the same name, but the new one has no association with the old
    subscription or its topic unless the same topic is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-delete-openapi.md
- name: Google Cloud Pub/Sub - Get Subscription
  x-api-slug: v1subscription-get
  description: Gets the configuration details of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-get-openapi.md
- name: Google Cloud Pub/Sub - Acknowledge Subscription
  x-api-slug: v1subscriptionacknowledge-post
  description: |-
    Acknowledges the messages associated with the `ack_ids` in the
    `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
    from the subscription.

    Acknowledging a message whose ack deadline has expired may succeed,
    but such a message may be redelivered later. Acknowledging a message more
    than once will not result in an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscriptionacknowledge-post-openapi.md
- name: Google Cloud Pub/Sub - Acknowledge Subscription
  x-api-slug: v1subscriptionacknowledge-post
  description: |-
    Acknowledges the messages associated with the `ack_ids` in the
    `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
    from the subscription.

    Acknowledging a message whose ack deadline has expired may succeed,
    but such a message may be redelivered later. Acknowledging a message more
    than once will not result in an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscriptionacknowledge-post-openapi.md
- name: Google Cloud Pub/Sub - Get Subscription
  x-api-slug: v1subscription-get
  description: Gets the configuration details of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-get-openapi.md
- name: Google Cloud Pub/Sub - Delete Subscription
  x-api-slug: v1subscription-delete
  description: |-
    Deletes an existing subscription. All messages retained in the subscription
    are immediately dropped. Calls to `Pull` after deletion will return
    `NOT_FOUND`. After a subscription is deleted, a new one may be created with
    the same name, but the new one has no association with the old
    subscription or its topic unless the same topic is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1subscription-delete-openapi.md
- name: Google Cloud Pub/Sub - List Matching Subscription
  x-api-slug: v1projectsubscriptions-get
  description: Lists matching subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/google-cloud-pub-sub/v1projectsubscriptions-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.prediction.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.pub.sub.stack.network
- type: x-change-log
  url: https://cloud.google.com/pubsub/docs/release-notes
- type: x-code
  url: https://cloud.google.com/pubsub/docs/reference/libraries
- type: x-faq
  url: https://cloud.google.com/pubsub/docs/faq
- type: x-getting-started
  url: https://cloud.google.com/pubsub/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/pubsub/docs/how-to
- type: x-issues
  url: https://issuetracker.google.com/issues?q=componentid:187173%20status:open
- type: x-pricing
  url: https://cloud.google.com/pubsub/pricing
- type: x-rate-limits
  url: https://cloud.google.com/pubsub/quotas
- type: x-service-level-agreement
  url: https://cloud.google.com/pubsub/sla
- type: x-support
  url: https://cloud.google.com/pubsub/docs/support
- type: x-website
  url: https://cloud.google.com/pubsub/docs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---