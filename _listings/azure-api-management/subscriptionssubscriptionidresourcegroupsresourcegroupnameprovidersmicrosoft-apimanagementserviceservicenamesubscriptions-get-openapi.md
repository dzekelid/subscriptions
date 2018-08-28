---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API Subscriptions List
  description: Lists all subscriptions of the API Management service instance.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/subscriptions
  : get:
      summary: Subscriptions List
      description: Lists all subscriptions of the API Management service instance.
      operationId: Subscriptions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamesubscriptions-get
      parameters:
      - in: query
        name: $filter
        description: '| Field        | Supported operators    | Supported functions                         ||--------------|------------------------|---------------------------------------------||
          id           | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || name         | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || stateComment | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || userId       | ge, le, eq, ne, gt, lt
          | substringof, contains, startswith, endswith || productId    | ge, le,
          eq, ne, gt, lt | substringof, contains, startswith, endswith || state        |
          eq                     |                                             |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
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