---
name: Azure API Management
x-slug: azure-api-management
description: Use Azure API Management as a turnkey solution for publishing APIs to
  external and internal customers. Quickly create consistent and modern API gateways
  for existing back-end services hosted anywhere, secure and protect them from abuse
  and overuse, and get insights into usage and health. Plus, automate and scale developer
  onboarding to help get your API program up and running.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Subscriptions
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/apis.md
specificationVersion: "0.14"
apis:
- name: Azure API Management API ProductSubscriptions ListByProducts
  x-api-slug: azure-api-management-api
  description: Lists the collection of subscriptions to the specified product.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/products/{productId}/subscriptions
  tags: Product Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameproductsproductidsubscriptions-get-openapi.md
- name: Azure API Management API Subscriptions List
  x-api-slug: azure-api-management-api
  description: Lists all subscriptions of the API Management service instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptions-get-openapi.md
- name: Azure API Management API Subscriptions Get
  x-api-slug: azure-api-management-api
  description: Gets the specified Subscription entity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssid-get-openapi.md
- name: Azure API Management API Subscriptions CreateOrUpdate
  x-api-slug: azure-api-management-api
  description: Creates or updates the subscription of specified user to the specified
    product.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssid-put-openapi.md
- name: Azure API Management API Subscriptions Update
  x-api-slug: azure-api-management-api
  description: Updates the details of a subscription specificied by its identifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssid-patch-openapi.md
- name: Azure API Management API Subscriptions Delete
  x-api-slug: azure-api-management-api
  description: Deletes the specified subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssid-delete-openapi.md
- name: Azure API Management API Subscriptions RegeneratePrimaryKey
  x-api-slug: azure-api-management-api
  description: Regenerates primary key of existing subscription of the API Management
    service instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}/regeneratePrimaryKey
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssidregenerateprimarykey-post-openapi.md
- name: Azure API Management API Subscriptions RegenerateSecondaryKey
  x-api-slug: azure-api-management-api
  description: Regenerates secondary key of existing subscription of the API Management
    service instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions/{sid}/regenerateSecondaryKey
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptionssidregeneratesecondarykey-post-openapi.md
- name: Azure API Management API
  x-api-slug: azure-api-management-api
  description: Use Azure API Management as a turnkey solution for publishing APIs
    to external and internal customers. Quickly create consistent and modern API gateways
    for existing back-end services hosted anywhere, secure and protect them from abuse
    and overuse, and get insights into usage and health. Plus, automate and scale
    developer onboarding to help get your API program up and running.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-api-management.png
  humanURL: https://azure.microsoft.com/en-us/services/api-management/
  baseURL: ://management.azure.com//
  tags: Subscriptions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/subscriptions/master/_listings/azure-api-management/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/api-management/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/api-management/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/api-management/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/api-management/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---