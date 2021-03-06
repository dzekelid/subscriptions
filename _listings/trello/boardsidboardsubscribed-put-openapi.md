---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Boards Subscribed
  description: Put boards subscribed.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/subscribed:
    put:
      summary: Put Boards Subscribed
      description: Put boards subscribed.
      operationId: updateBoardsSubscribedByIdBoard
      x-api-path-slug: boardsidboardsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Subscribed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Subscribed
  /cards/{idCard}/subscribed:
    put:
      summary: Put Cards Subscribed
      description: Put cards subscribed.
      operationId: updateCardsSubscribedByIdCard
      x-api-path-slug: cardsidcardsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Subscribed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Subscribed
  /lists/{idList}/subscribed:
    put:
      summary: Put Lists List Subscribed
      description: Put lists list subscribed.
      operationId: updateListsSubscribedByIdList
      x-api-path-slug: listsidlistsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Subscribed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Subscribed
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