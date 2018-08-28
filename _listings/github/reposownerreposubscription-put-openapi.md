---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Put Repos Owner Repo Subscription
  description: Set a Repository Subscription
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/subscriptions:
    get:
      summary: Get User Subscriptions
      description: List repositories being watched by the authenticated user.
      operationId: list-repositories-being-watched-by-the-authenticated-user
      x-api-path-slug: usersubscriptions-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - User
      - Subscriptions
  /user/subscriptions/{owner}/{repo}:
    delete:
      summary: Delete User Subscriptions Owner Repo
      description: Stop watching a repository
      operationId: stop-watching-a-repository
      x-api-path-slug: usersubscriptionsownerrepo-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of the owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - User
      - Subscriptions
      - Owner
      - Repo
    get:
      summary: Get User Subscriptions Owner Repo
      description: Check if you are watching a repository.
      operationId: check-if-you-are-watching-a-repository
      x-api-path-slug: usersubscriptionsownerrepo-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of the owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - User
      - Subscriptions
      - Owner
      - Repo
    put:
      summary: Put User Subscriptions Owner Repo
      description: Watch a repository.
      operationId: watch-a-repository
      x-api-path-slug: usersubscriptionsownerrepo-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of the owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - User
      - Subscriptions
      - Owner
      - Repo
  /users/{username}/subscriptions:
    get:
      summary: Get Users Username Subscriptions
      description: List repositories being watched by a user.
      operationId: list-repositories-being-watched-by-a-user
      x-api-path-slug: usersusernamesubscriptions-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Subscriptions
  /notifications/threads/{id}/subscription:
    delete:
      summary: Delete Notifications Threads  Subscription
      description: Delete a Thread Subscription.
      operationId: delete-a-thread-subscription
      x-api-path-slug: notificationsthreadsidsubscription-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
        description: Id of thread
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Threads
      - ""
      - Subscription
    get:
      summary: Get Notifications Threads  Subscription
      description: Get a Thread Subscription.
      operationId: get-a-thread-subscription
      x-api-path-slug: notificationsthreadsidsubscription-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
        description: Id of thread
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Threads
      - ""
      - Subscription
    put:
      summary: Put Notifications Threads  Subscription
      description: |-
        Set a Thread Subscription.
        This lets you subscribe to a thread, or ignore it. Subscribing to a thread
        is unnecessary if the user is already subscribed to the repository. Ignoring
        a thread will mute all future notifications (until you comment or get @mentioned).
      operationId: set-a-thread-subscriptionthis-lets-you-subscribe-to-a-thread-or-ignore-it-subscribing-to-a-threadis-
      x-api-path-slug: notificationsthreadsidsubscription-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of thread
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Threads
      - ""
      - Subscription
  /repos/{owner}/{repo}/subscription:
    delete:
      summary: Delete Repos Owner Repo Subscription
      description: Delete a Repository Subscription.
      operationId: delete-a-repository-subscription
      x-api-path-slug: reposownerreposubscription-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Subscription
    get:
      summary: Get Repos Owner Repo Subscription
      description: Get a Repository Subscription.
      operationId: get-a-repository-subscription
      x-api-path-slug: reposownerreposubscription-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Subscription
    put:
      summary: Put Repos Owner Repo Subscription
      description: Set a Repository Subscription
      operationId: set-a-repository-subscription
      x-api-path-slug: reposownerreposubscription-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Subscription
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