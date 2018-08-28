swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tracking_settings/subscription:
    get:
      summary: Get Tracking Settings Subscription
      description: |-
        **This endpoint allows you to retrieve your current settings for subscription tracking.**

        Subscription tracking adds links to the bottom of your emails that allows your recipients to subscribe to, or unsubscribe from, your emails.

        You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

        For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
      operationId: tracking_settings.subscription.get
      x-api-path-slug: tracking-settingssubscription-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Tracking
      - Settings
      - Subscription
    patch:
      summary: Patch Tracking Settings Subscription
      description: |-
        **This endpoint allows you to update your current settings for subscription tracking.**

        Subscription tracking adds links to the bottom of your emails that allows your recipients to subscribe to, or unsubscribe from, your emails.

        You can track a variety of the actions your recipients may take when interacting with your emails including opening your emails, clicking on links in your emails, and subscribing to (or unsubscribing from) your emails.

        For more information about tracking, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/tracking.html).
      operationId: tracking_settings.subscription.patch
      x-api-path-slug: tracking-settingssubscription-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Tracking
      - Settings
      - Subscription