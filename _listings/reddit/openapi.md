swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscribe:
    post&nbsp;:
      summary: Add Subscribe
      description: Subscribe to or unsubscribe from a subreddit.
      operationId: post&nbsp;Subscribe
      x-api-path-slug: subscribe-postnbsp
      parameters:
      - in: query
        name: action
        description: one of (sub, unsub)
        type: string
      - in: query
        name: skip_initial_defaults
        description: boolean value
        type: string
      - in: query
        name: sr / sr_name
        description: A comma-separated list of subreddit fullnames (when using the
          &quot;sr&quot; parameter), or of subreddit names (when using the &quot;sr_name&quot;
          parameter)
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscribe