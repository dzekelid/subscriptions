swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/merge_request/{subscribable_id}/subscription:
    post:
      summary: Post Projects Merge Request Subscribable Subscription
      description: Post projects merge request subscribable subscription.
      operationId: postV3ProjectsIdMergeRequestSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestsubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Merge Request Subscribable Subscription
      description: Delete projects merge request subscribable subscription.
      operationId: deleteV3ProjectsIdMergeRequestSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestsubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Subscribable
      - Subscription
  /v3/projects/{id}/merge_requests/{subscribable_id}/subscription:
    post:
      summary: Post Projects Merge Requests Subscribable Subscription
      description: Post projects merge requests subscribable subscription.
      operationId: postV3ProjectsIdMergeRequestsSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestssubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Merge Requests Subscribable Subscription
      description: Delete projects merge requests subscribable subscription.
      operationId: deleteV3ProjectsIdMergeRequestsSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestssubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Subscribable
      - Subscription
  /v3/projects/{id}/issues/{subscribable_id}/subscription:
    post:
      summary: Post Projects Issues Subscribable Subscription
      description: Post projects issues subscribable subscription.
      operationId: postV3ProjectsIdIssuesSubscribableIdSubscription
      x-api-path-slug: v3projectsidissuessubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Issues Subscribable Subscription
      description: Delete projects issues subscribable subscription.
      operationId: deleteV3ProjectsIdIssuesSubscribableIdSubscription
      x-api-path-slug: v3projectsidissuessubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Subscribable
      - Subscription
  /v3/projects/{id}/labels/{subscribable_id}/subscription:
    post:
      summary: Post Projects Labels Subscribable Subscription
      description: Post projects labels subscribable subscription.
      operationId: postV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Labels Subscribable Subscription
      description: Delete projects labels subscribable subscription.
      operationId: deleteV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription