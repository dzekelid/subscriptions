swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/event_comment_subscribe/:id:
    post:
      summary: Event Comment Subscribe
      description: Subscribe to notifications on updates to a given comment thread
      operationId: events
      x-api-path-slug: 2event-comment-subscribeid-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ratings