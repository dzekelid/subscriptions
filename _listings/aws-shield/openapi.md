swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 1
info:
  title: AWS Shield API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeSubscription:
    get:
      summary: Describe Subscription
      description: Provides details about the AWS Shield Advanced subscription for
        an account.
      operationId: describeSubscription
      x-api-path-slug: actiondescribesubscription-get
      parameters:
      - in: query
        name: Subscription
        description: The AWS Shield Advanced subscription details for an account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=CreateSubscription:
    get:
      summary: Create Subscription
      description: Activates AWS Shield Advanced for an account.
      operationId: createSubscription
      x-api-path-slug: actioncreatesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DeleteSubscription:
    get:
      summary: Delete Subscription
      description: Removes AWS Shield Advanced from an account.
      operationId: deleteSubscription
      x-api-path-slug: actiondeletesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection