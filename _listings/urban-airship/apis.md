---
name: Urban Airship
x-slug: urban-airship
description: A market-leading mobile app engagement, mobile analytics, mobile data
  integration and mobile wallet marketing solution.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
x-kinRank: "8"
x-alexaRank: "76944"
tags: Subscriptions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/apis.md
specificationVersion: "0.14"
apis:
- name: Urban Airship Get User User Available Subscriptions
  x-api-slug: urban-airship
  description: Retrieves subscription options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api///user/{user_id}/available_subscriptions
  tags: User,User,Id,Available,Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idavailable-subscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idavailable-subscriptions-get-openapi.md
- name: Urban Airship Post User User Subscriptions Subscription Key Purchase
  x-api-slug: urban-airship
  description: Adds a new subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api///user/{user_id}/subscriptions/{subscription_key}/purchase
  tags: User,User,Id,Subscriptions,Subscription,Key,Purchase
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idsubscriptionssubscription-keypurchase-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idsubscriptionssubscription-keypurchase-post-openapi.md
- name: Urban Airship Post User User Subscriptions Content Content Download
  x-api-slug: urban-airship
  description: Downloads the content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api///user/{user_id}/subscriptions/content/{content_id}/download
  tags: User,User,Id,Subscriptions,Content,Content,Id,Download
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idsubscriptionscontentcontent-iddownload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/useruser-idsubscriptionscontentcontent-iddownload-post-openapi.md
- name: Urban Airship
  x-api-slug: urban-airship
  description: The Urban Airship Push API is a major update which unifies several
    legacy endpoints into two&mdash; one for sending messages and one for scheduling.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/urban-airship/openapi.md
x-common:
- type: x-website
  url: http://urbanairship.com/
- type: x-android-sdk
  url: http://docs.urbanairship.com/platform/android.html
- type: x-blackberry-sdk
  url: http://docs.urbanairship.com/platform/blackberry.html
- type: x-blog
  url: http://urbanairship.com/blog
- type: x-blog-rss
  url: http://urbanairship.com/blog/rss
- type: x-case-studies
  url: http://urbanairship.com/resources/case-studies
- type: x-crunchbase
  url: http://www.crunchbase.com/company/urban-airship
- type: x-crunchbase
  url: https://crunchbase.com/organization/urban-airship
- type: x-developer
  url: http://docs.urbanairship.com/
- type: x-email
  url: legal@urbanairship.com
- type: x-email
  url: privacy@urbanairship.com
- type: x-email
  url: support@urbanairship.com
- type: x-github
  url: https://github.com/urbanairship
- type: x-glossary
  url: http://docs.urbanairship.com/reference/glossary.html
- type: x-ios-sdk
  url: http://docs.urbanairship.com/platform/ios.html
- type: x-phonegap-sdk
  url: http://docs.urbanairship.com/platform/phonegap.html
- type: x-pricing
  url: https://www.urbanairship.com/products/engage/pricing
- type: x-privacy
  url: http://urbanairship.com/legal/privacy-policy
- type: x-security
  url: http://docs.urbanairship.com/reference/app_keys_secrets.html
- type: x-twitter
  url: https://twitter.com/urbanairship
- type: x-website
  url: http://urbanairship.com
- type: x-white-papers
  url: http://urbanairship.com/resources/whitepapers
- type: x-windows-sdk
  url: http://docs.urbanairship.com/platform/windows.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---