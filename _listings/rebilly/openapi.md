swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions:
    get:
      summary: Retrieve a list of subscriptions
      description: Retrieve a list of subscriptions
      operationId: subscriptions.get
      x-api-path-slug: subscriptions-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Subscriptions
    post:
      summary: Create a subscription
      description: Create a subscription
      operationId: subscriptions.post
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: body
        description: Subscription resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /subscriptions/{id}/lead-source:
    get:
      summary: Retrieve a subscription's Lead Source
      description: Retrieve a Lead Source of given subscription
      operationId: subscriptions.id.lead_source.get
      x-api-path-slug: subscriptionsidleadsource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Subscriptions
      - Lead
      - Source
    delete:
      summary: Delete a Lead Source for a Subscription
      description: Delete a Lead Source that belongs to a certain Subscription
      operationId: subscriptions.id.lead_source.delete
      x-api-path-slug: subscriptionsidleadsource-delete
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Subscription
    put:
      summary: Create a Lead Source for a Subscription
      description: Create a Lead Source for a Subscription
      operationId: subscriptions.id.lead_source.put
      x-api-path-slug: subscriptionsidleadsource-put
      parameters:
      - in: body
        name: body
        description: Lead Source resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Lead
      - Sourcea
      - Subscription
  /subscriptions/{id}:
    get:
      summary: Retrieve a subscription
      description: Retrieve a subscription with specified identifier string
      operationId: subscriptions.id.get
      x-api-path-slug: subscriptionsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Subscription
    put:
      summary: Create or update a subscription with predefined ID
      description: Create or update a subscription with predefined identifier string
      operationId: subscriptions.id.put
      x-api-path-slug: subscriptionsid-put
      parameters:
      - in: body
        name: body
        description: Subscription resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Subscription
      - Predefined
      - ID
  /subscriptions/{id}/cancel:
    post:
      summary: Cancel a subscription
      description: Cancel a subscription
      operationId: subscriptions.id.cancel.post
      x-api-path-slug: subscriptionsidcancel-post
      parameters:
      - in: body
        name: body
        description: Only policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription
  /subscriptions/{id}/matched-rules:
    get:
      summary: Get matched rules for the subscription
      description: Get matched rules for the subscription
      operationId: subscriptions.id.matched_rules.get
      x-api-path-slug: subscriptionsidmatchedrules-get
      responses:
        200:
          description: OK
      tags:
      - Matched
      - Rulesthe
      - Subscription
  /subscriptions/{id}/switch:
    post:
      summary: Switch a subscription
      description: Switch a subscription
      operationId: subscriptions.id.switch.post
      x-api-path-slug: subscriptionsidswitch-post
      parameters:
      - in: body
        name: body
        description: SubscriptionSwitch resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Subscription
  /tracking/subscriptions:
    get:
      summary: Retrieve a list of tracking subscription logs
      description: ""
      operationId: ""
      x-api-path-slug: trackingsubscriptions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tracking
      - Subscription
      - Logs
  /tracking/subscriptions/{id}:
    get:
      summary: Retrieve a tracking subscription log with specified identifier string
      description: ""
      operationId: ""
      x-api-path-slug: trackingsubscriptionsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Tracking
      - Subscription
      - Log
      - Specified
      - Identifier
      - String