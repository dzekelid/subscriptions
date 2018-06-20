---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Partner
  version: "1.0"
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /offers/fares/subscriptions:
    get:
      summary: Fares Subscriptions
      description: Create a subscription for best price O&D. Receive regular updates
        on lowest fares
      operationId: offers.fares.subscriptions.get
      x-api-path-slug: offersfaressubscriptions-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: cabin-class
        description: 'Cabin class: economy, premium_economy, business, first (Acceptable
          values are: , economy, premium_economy, business, first)'
      - in: query
        name: country
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: destination
        description: Journey destination
      - in: query
        name: email
        description: Email Address)
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: origin
        description: Journey origin
      - in: query
        name: trackingid
        description: Tracking parameter
      - in: query
        name: trip-duration
        description: Trip duration in days (e
      responses:
        200:
          description: OK
      tags:
      - Fares
      - Subscriptions
---