---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripes payment platform to accept
  and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1914"
tags: Subscriptions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe - Get Customers Customer Subscriptions
  x-api-slug: customerscustomersubscriptions-get
  description: You can see a list of the customer???s active subscriptions. Note that
    the 10 most recent active subscriptions are always available by default on the
    customer object. If you need more than those 10, you can use the limit and starting_after
    parameters to page through additional subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-get-openapi.md
- name: Stripe - Add Customers Customer Subscriptions
  x-api-slug: customerscustomersubscriptions-post
  description: Creates a new subscription on an existing customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-post-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-delete
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Get Subscriptions
  x-api-slug: subscriptions-get
  description: By default, returns a list of subscriptions that have not been canceled.
    In order to list canceled subscriptions, specify status=canceled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptions-get-openapi.md
- name: Stripe - Add Subscriptions
  x-api-slug: subscriptions-post
  description: Creates a new subscription on an existing customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptions-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-get
  description: Retrieves the subscription with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed  Discount
  x-api-slug: subscriptionssubscription-exposed-iddiscount-delete
  description: Delete Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-delete
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Get Subscription Items
  x-api-slug: subscription-items-get
  description: Returns a list of your subscription items for a given subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-get-openapi.md
- name: Stripe - Add Subscription Items
  x-api-slug: subscription-items-post
  description: Adds a new item to an existing subscription. No existing items will
    be changed or replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-post-openapi.md
- name: Stripe - Delete Subscription Items Item
  x-api-slug: subscription-itemsitem-delete
  description: Deletes an item from the subscription. Removing a subscription item
    from a subscription will not cancel the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-delete-openapi.md
- name: Stripe - Get Subscription Items Item
  x-api-slug: subscription-itemsitem-get
  description: Retrieves the invoice item with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-get-openapi.md
- name: Stripe - Add Subscription Items Item
  x-api-slug: subscription-itemsitem-post
  description: Updates the plan or quantity of an item on a current subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-get
  description: Retrieves the subscription with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed  Discount
  x-api-slug: subscriptionssubscription-exposed-iddiscount-delete
  description: Delete Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-delete
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Get Subscription Items
  x-api-slug: subscription-items-get
  description: Returns a list of your subscription items for a given subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-get-openapi.md
- name: Stripe - Add Subscription Items
  x-api-slug: subscription-items-post
  description: Adds a new item to an existing subscription. No existing items will
    be changed or replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-post-openapi.md
- name: Stripe - Delete Subscription Items Item
  x-api-slug: subscription-itemsitem-delete
  description: Deletes an item from the subscription. Removing a subscription item
    from a subscription will not cancel the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-delete-openapi.md
- name: Stripe - Get Subscription Items Item
  x-api-slug: subscription-itemsitem-get
  description: Retrieves the invoice item with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-get-openapi.md
- name: Stripe - Add Subscription Items Item
  x-api-slug: subscription-itemsitem-post
  description: Updates the plan or quantity of an item on a current subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Get Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-get
  description: Retrieves the subscription with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Add Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed  Discount
  x-api-slug: subscriptionssubscription-exposed-iddiscount-delete
  description: Delete Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed  Discount
  x-api-slug: subscriptionssubscription-exposed-iddiscount-delete
  description: Delete Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Add Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Get Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-get
  description: Retrieves the subscription with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Delete Subscriptions Subscription Exposed
  x-api-slug: subscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe - Add Subscription Items Item
  x-api-slug: subscription-itemsitem-post
  description: Updates the plan or quantity of an item on a current subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-post-openapi.md
- name: Stripe - Get Subscription Items Item
  x-api-slug: subscription-itemsitem-get
  description: Retrieves the invoice item with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-get-openapi.md
- name: Stripe - Delete Subscription Items Item
  x-api-slug: subscription-itemsitem-delete
  description: Deletes an item from the subscription. Removing a subscription item
    from a subscription will not cancel the subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-itemsitem-delete-openapi.md
- name: Stripe - Add Subscription Items
  x-api-slug: subscription-items-post
  description: Adds a new item to an existing subscription. No existing items will
    be changed or replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-post-openapi.md
- name: Stripe - Get Subscription Items
  x-api-slug: subscription-items-get
  description: Returns a list of your subscription items for a given subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscription-items-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-delete
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe - Add Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-post
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Delete Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-delete
  description: Cancels a customer???s subscription. If you set the at_period_end parameter
    to true, the subscription will remain active until the end of the period, at which
    point it will be canceled and not renewed. By default, the subscription is terminated
    immediately. In either case, the customer will not be charged again for the subscription.
    Note, however, that any pending invoice items that you???ve created will still
    be charged for at the end of the period unless manually deleted. If you???ve set
    the subscription to cancel at period end, any pending prorations will also be
    left in place and collected at the end of the period, but if the subscription
    is set to cancel immediately, pending prorations will be removed.By default, all
    unpaid invoices for the customer will be closed upon subscription cancellation.
    We do this in order to prevent unexpected payment attempts once the customer has
    canceled a subscription. However, you can reopen the invoices manually after subscription
    cancellation to have us proceed with payment collection, or you could even re-attempt
    payment yourself on all unpaid invoices before allowing the customer to cancel
    the subscription at all.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://stride.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stripe.stack.network
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-email
  url: dpo@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-linkedin
  url: https://www.linkedin.com/company/stripe/
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---