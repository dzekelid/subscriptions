---
swagger: "2.0"
x-collection-name: Stripe
x-complete: 0
info:
  title: Stripe Delete Customers Customer Subscriptions Subscription Exposed  Discount
  description: Delete Customers, Customer, Subscriptions, Subscription, Exposed, ,
    Discount
  termsOfService: https://stripe.com/us/terms/
  contact:
    name: Stripe Dev Platform Team
    url: https://stripe.com
    email: dev-platform@stripe.com
  version: v1
host: api.stripe.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers/{customer}/subscriptions:
    get:
      summary: Get Customers Customer Subscriptions
      description: "You can see a list of the customer\u2019s active subscriptions.
        Note that the 10 most recent active subscriptions are always available by
        default on the customer object. If you need more than those 10, you can use
        the limit and starting_after parameters to page through additional subscriptions."
      operationId: getCustomersCustomerSubscriptions
      x-api-path-slug: customerscustomersubscriptions-get
      parameters:
      - in: path
        name: customer
        description: The ID of the customer whose subscriptions will be retrieved
      - in: query
        name: ending_before
        description: A cursor for use in pagination
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: query
        name: limit
        description: A limit on the number of objects to be returned
      - in: query
        name: starting_after
        description: A cursor for use in pagination
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
    post:
      summary: Add Customers Customer Subscriptions
      description: Creates a new subscription on an existing customer.
      operationId: postCustomersCustomerSubscriptions
      x-api-path-slug: customerscustomersubscriptions-post
      parameters:
      - in: path
        name: customer
        description: The identifier of the customer to subscribe
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
  /customers/{customer}/subscriptions/{subscription_exposed_id}:
    delete:
      summary: Delete Customers Customer Subscriptions Subscription Exposed
      description: "Cancels a customer\u2019s subscription. If you set the at_period_end
        parameter to true, the subscription will remain active until the end of the
        period, at which point it will be canceled and not renewed. By default, the
        subscription is terminated immediately. In either case, the customer will
        not be charged again for the subscription. Note, however, that any pending
        invoice items that you\u2019ve created will still be charged for at the end
        of the period unless manually deleted. If you\u2019ve set the subscription
        to cancel at period end, any pending prorations will also be left in place
        and collected at the end of the period, but if the subscription is set to
        cancel immediately, pending prorations will be removed.By default, all unpaid
        invoices for the customer will be closed upon subscription cancellation. We
        do this in order to prevent unexpected payment attempts once the customer
        has canceled a subscription. However, you can reopen the invoices manually
        after subscription cancellation to have us proceed with payment collection,
        or you could even re-attempt payment yourself on all unpaid invoices before
        allowing the customer to cancel the subscription at all."
      operationId: deleteCustomersCustomerSubscriptionsSubscriptionExposed
      x-api-path-slug: customerscustomersubscriptionssubscription-exposed-id-delete
      parameters:
      - in: path
        name: customer
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription_exposed_id
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
      - Subscription
      - Exposed
    get:
      summary: Get Customers Customer Subscriptions Subscription Exposed
      description: Get Customers, Customer, Subscriptions, Subscription, Exposed
      operationId: getCustomersCustomerSubscriptionsSubscriptionExposed
      x-api-path-slug: customerscustomersubscriptionssubscription-exposed-id-get
      parameters:
      - in: path
        name: customer
      - in: query
        name: expand
        description: Specifies which fields in the response should be expanded
      - in: path
        name: subscription_exposed_id
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
      - Subscription
      - Exposed
    post:
      summary: Add Customers Customer Subscriptions Subscription Exposed
      description: Updates an existing subscription on a customer to match the specified
        parameters. When changing plans or quantities, we will optionally prorate
        the price we charge next month to make up for any price changes. To preview
        how the proration will be calculated, use the upcoming invoice endpoint.
      operationId: postCustomersCustomerSubscriptionsSubscriptionExposed
      x-api-path-slug: customerscustomersubscriptionssubscription-exposed-id-post
      parameters:
      - in: path
        name: customer
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription_exposed_id
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
      - Subscription
      - Exposed
  /customers/{customer}/subscriptions/{subscription_exposed_id}/discount:
    delete:
      summary: Delete Customers Customer Subscriptions Subscription Exposed  Discount
      description: Delete Customers, Customer, Subscriptions, Subscription, Exposed,
        , Discount
      operationId: deleteCustomersCustomerSubscriptionsSubscriptionExposedDiscount
      x-api-path-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-delete
      parameters:
      - in: path
        name: customer
      - in: body
        name: payload
        description: Body parameters for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription_exposed_id
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Customers
      - Customer
      - Subscriptions
      - Subscription
      - Exposed
      - ""
      - Discount
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---