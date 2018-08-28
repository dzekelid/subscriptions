---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Describe Spot Datafeed Subscription
  version: 1.0.0
  description: Describes the data feed for Spot instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateSpotDatafeedSubscription:
    get:
      summary: Create Spot Datafeed Subscription
      description: Creates a data feed for Spot instances, enabling you to view Spot
        instance usage logs.
      operationId: createspotdatafeedsubscription
      x-api-path-slug: actioncreatespotdatafeedsubscription-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=DeleteSpotDatafeedSubscription:
    get:
      summary: Delete Spot Datafeed Subscription
      description: Deletes the data feed for Spot instances.
      operationId: deletespotdatafeedsubscription
      x-api-path-slug: actiondeletespotdatafeedsubscription-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Data Feed Subscription
  /?Action=DescribeSpotDatafeedSubscription:
    get:
      summary: Describe Spot Datafeed Subscription
      description: Describes the data feed for Spot instances.
      operationId: describespotdatafeedsubscription
      x-api-path-slug: actiondescribespotdatafeedsubscription-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: SpotInstanceRequestId.N
        description: One or more Spot instance request IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Data Feed
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