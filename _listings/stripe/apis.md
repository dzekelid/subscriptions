---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripe???s payment platform to
  accept and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1793"
tags: Subscriptions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Get Customers Customer Subscriptions
  x-api-slug: stripe
  description: "You can see a list of the customer\u2019s active subscriptions. Note
    that the 10 most recent active subscriptions are always available by default on
    the customer object. If you need more than those 10, you can use the limit and
    starting_after parameters to page through additional subscriptions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions
  tags: Customers, Customer, Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-get-openapi.md
- name: Stripe Add Customers Customer Subscriptions
  x-api-slug: stripe
  description: Creates a new subscription on an existing customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions
  tags: Customers, Customer, Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptions-post-openapi.md
- name: Stripe Delete Customers Customer Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: "Cancels a customer\u2019s subscription. If you set the at_period_end
    parameter to true, the subscription will remain active until the end of the period,
    at which point it will be canceled and not renewed. By default, the subscription
    is terminated immediately. In either case, the customer will not be charged again
    for the subscription. Note, however, that any pending invoice items that you\u2019ve
    created will still be charged for at the end of the period unless manually deleted.
    If you\u2019ve set the subscription to cancel at period end, any pending prorations
    will also be left in place and collected at the end of the period, but if the
    subscription is set to cancel immediately, pending prorations will be removed.By
    default, all unpaid invoices for the customer will be closed upon subscription
    cancellation. We do this in order to prevent unexpected payment attempts once
    the customer has canceled a subscription. However, you can reopen the invoices
    manually after subscription cancellation to have us proceed with payment collection,
    or you could even re-attempt payment yourself on all unpaid invoices before allowing
    the customer to cancel the subscription at all."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions/{subscription_exposed_id}
  tags: Customers, Customer, Subscriptions, Subscription, Exposed
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions/{subscription_exposed_id}
  tags: Customers, Customer, Subscriptions, Subscription, Exposed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe Add Customers Customer Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions/{subscription_exposed_id}
  tags: Customers, Customer, Subscriptions, Subscription, Exposed
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe Delete Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: stripe
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions/{subscription_exposed_id}/discount
  tags: Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: stripe
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///customers/{customer}/subscriptions/{subscription_exposed_id}/discount
  tags: Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe Get Subscriptions
  x-api-slug: stripe
  description: By default, returns a list of subscriptions that have not been canceled.
    In order to list canceled subscriptions, specify status=canceled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptions-get-openapi.md
- name: Stripe Add Subscriptions
  x-api-slug: stripe
  description: Creates a new subscription on an existing customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptions-post-openapi.md
- name: Stripe Delete Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: "Cancels a customer\u2019s subscription. If you set the at_period_end
    parameter to true, the subscription will remain active until the end of the period,
    at which point it will be canceled and not renewed. By default, the subscription
    is terminated immediately. In either case, the customer will not be charged again
    for the subscription. Note, however, that any pending invoice items that you\u2019ve
    created will still be charged for at the end of the period unless manually deleted.
    If you\u2019ve set the subscription to cancel at period end, any pending prorations
    will also be left in place and collected at the end of the period, but if the
    subscription is set to cancel immediately, pending prorations will be removed.By
    default, all unpaid invoices for the customer will be closed upon subscription
    cancellation. We do this in order to prevent unexpected payment attempts once
    the customer has canceled a subscription. However, you can reopen the invoices
    manually after subscription cancellation to have us proceed with payment collection,
    or you could even re-attempt payment yourself on all unpaid invoices before allowing
    the customer to cancel the subscription at all."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions/{subscription_exposed_id}
  tags: Subscriptions, Subscription, Exposed
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-delete-openapi.md
- name: Stripe Get Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: Retrieves the subscription with the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions/{subscription_exposed_id}
  tags: Subscriptions, Subscription, Exposed
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe Add Subscriptions Subscription Exposed
  x-api-slug: stripe
  description: Updates an existing subscription on a customer to match the specified
    parameters. When changing plans or quantities, we will optionally prorate the
    price we charge next month to make up for any price changes. To preview how the
    proration will be calculated, use the upcoming invoice endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions/{subscription_exposed_id}
  tags: Subscriptions, Subscription, Exposed
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-id-post-openapi.md
- name: Stripe Delete Subscriptions Subscription Exposed  Discount
  x-api-slug: stripe
  description: Delete Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///subscriptions/{subscription_exposed_id}/discount
  tags: Subscriptions, Subscription, Exposed, , Discount
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/subscriptionssubscription-exposed-iddiscount-delete-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/stripe/openapi.md
x-common:
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
- type: x-github
  url: https://github.com/stripe
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