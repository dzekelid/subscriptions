---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Nurego Parameters Subscriptions Entitlements
  description: Parameters subscriptions entitlements.
  contact:
    name: support@nurego.com
  version: 1.0.0
host: api.nurego.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/subscriptions/{subscription_id}:
    parameters:
      summary: Parameters Subscriptions
      description: Parameters subscriptions.
      operationId: parametersV1SubscriptionsSubscription
      x-api-path-slug: v1subscriptionssubscription-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Subscriptions
    get:
      summary: Get Subscriptions
      description: You can retrieve a specific subscription by using it's id.
      operationId: getV1SubscriptionsSubscription
      x-api-path-slug: v1subscriptionssubscription-id-get
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /v1/organizations/{organization_id}/subscriptions:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptions
      x-api-path-slug: v1organizationsorganization-idsubscriptions-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
    post:
      summary: Post Organizations Subscriptions
      description: Create a new subscription to a plan.
      operationId: postV1OrganizationsOrganizationSubscriptions
      x-api-path-slug: v1organizationsorganization-idsubscriptions-post
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions
  /v1/organizations/{organization_id}/subscriptions/{subscription_id}:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
    put:
      summary: Put Organizations Subscriptions
      description: You can update a subscription's plan, using the following parameters.
      operationId: putV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-put
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions
    delete:
      summary: Delete Organizations Subscriptions
      description: You can cancel a plan subscription using the following parameters.
        When the last subscription is canceled, the customer will become canceled.
      operationId: deleteV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-delete
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions
  /v1/subscriptions/{subscription_id}/entitlements:
    parameters:
      summary: Parameters Subscriptions Entitlements
      description: Parameters subscriptions entitlements.
      operationId: parametersV1SubscriptionsSubscriptionEntitlements
      x-api-path-slug: v1subscriptionssubscription-identitlements-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Subscriptions
      - Entitlements
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