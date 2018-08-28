---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Subscribe to a topic
  description: Subscribe to a topic.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/discussion_topics/topic_id/subscribed:
    delete:
      summary: Unsubscribe from a topic
      description: Unsubscribe from a topic.
      operationId: unsubscribe-from-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idsubscribed-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
    put:
      summary: Subscribe to a topic
      description: Subscribe to a topic.
      operationId: subscribe-to-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idsubscribed-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
  /groups/{group_id}/discussion_topics/topic_id/subscribed:
    delete:
      summary: Unsubscribe from a topic
      description: Unsubscribe from a topic.
      operationId: unsubscribe-from-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
    put:
      summary: Subscribe to a topic
      description: Subscribe to a topic.
      operationId: subscribe-to-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
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