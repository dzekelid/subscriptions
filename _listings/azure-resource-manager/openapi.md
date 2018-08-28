swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 1
info:
  title: SubscriptionClient
  description: all-resource-groups-and-resources-exist-within-subscriptions--these-operation-enable-you-get-information-about-your-subscriptions-and-tenants--a-tenant-is-a-dedicated-instance-of-azure-active-directory-azure-ad-for-your-organization-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}:
    get:
      summary: Subscriptions Get
      description: Gets details about a specified subscription.
      operationId: Subscriptions_Get
      x-api-path-slug: subscriptionssubscriptionid-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: subscriptionId
        description: The ID of the target subscription
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /subscriptions:
    get:
      summary: Subscriptions List
      description: Gets all subscriptions for a tenant.
      operationId: Subscriptions_List
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Subscriptions