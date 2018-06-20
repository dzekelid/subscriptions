---
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
---