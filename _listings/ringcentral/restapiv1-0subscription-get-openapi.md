---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Subscriptions
  description: |-
    Returns a list of subscriptions created by a particular user on a particular client app.
    Usage Plan Group
    Light
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/subscription:
    get:
      summary: Get Subscriptions
      description: |-
        Returns a list of subscriptions created by a particular user on a particular client app.
        Usage Plan Group
        Light
      operationId: listSubscriptions
      x-api-path-slug: restapiv1-0subscription-get
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