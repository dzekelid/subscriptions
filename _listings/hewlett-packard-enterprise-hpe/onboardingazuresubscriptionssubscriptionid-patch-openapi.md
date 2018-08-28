---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Patch Onboarding Azure Subscriptions Subscriptionid
  description: Updates a subscription
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /onboarding/azure/subscriptions:
    get:
      summary: Get Onboarding Azure Subscriptions
      description: Returns a list of Azure subscriptions and their display names
      operationId: ListAzureSubscriptions
      x-api-path-slug: onboardingazuresubscriptions-get
      parameters:
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Subscriptions
  /onboarding/azure/subscriptions/{subscriptionId}:
    patch:
      summary: Patch Onboarding Azure Subscriptions Subscriptionid
      description: Updates a subscription
      operationId: UpdateSubscription
      x-api-path-slug: onboardingazuresubscriptionssubscriptionid-patch
      parameters:
      - in: body
        name: body
        description: Update subscription
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: directoryUri
        description: The Azure Directory URI associated with the SubscriptionFor Example:myActiveDirectory
      - in: query
        name: location
        description: The full response Azure sends to the redirectURI including valid
          Azure authentication codeFor Example:https://customername
      - in: path
        name: subscriptionId
        description: The Azure subscriptionId
      responses:
        200:
          description: OK
      tags:
      - Onboarding
      - Azure
      - Subscriptions
      - Subscriptionid
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