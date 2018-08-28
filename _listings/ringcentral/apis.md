---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: Subscriptions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Get Subscriptions
  x-api-slug: restapiv1-0subscription-get
  description: |-
    Returns a list of subscriptions created by a particular user on a particular client app.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscription-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Subscription
  x-api-slug: restapiv1-0subscription-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscription-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-get
  description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription / Update Event
    Filters
  x-api-slug: restapiv1-0subscriptionsubscriptionid-put
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-delete
  description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Subscription
  x-api-slug: restapiv1-0subscription-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscription-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-get
  description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription / Update Event
    Filters
  x-api-slug: restapiv1-0subscriptionsubscriptionid-put
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-delete
  description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-delete
  description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-delete
  description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription / Update Event
    Filters
  x-api-slug: restapiv1-0subscriptionsubscriptionid-put
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-get
  description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-get
  description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Subscription
  x-api-slug: restapiv1-0subscription-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscription-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Subscription
  x-api-slug: restapiv1-0subscription-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/ringcentral/restapiv1-0subscription-post-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---