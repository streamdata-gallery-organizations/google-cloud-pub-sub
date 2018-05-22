---
swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 0
info:
  title: Google Cloud Pub/Sub API Get IAM Policy
  description: |-
    Gets the access control policy for a resource.
    Returns an empty policy if the resource exists and does not have a policy
    set.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: pubsub.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    put:
      summary: Create Topic
      description: Creates the given topic with the given name.
      operationId: pubsub.projects.topics.create
      x-api-path-slug: v1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the topic
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{project}/subscriptions:
    get:
      summary: List Matching Subscription
      description: Lists matching subscriptions.
      operationId: pubsub.projects.subscriptions.list
      x-api-path-slug: v1projectsubscriptions-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of subscriptions to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListSubscriptionsResponse`; indicates
          thatthis is a continuation of a prior `ListSubscriptions` call, and that
          thesystem should return the next page of data
      - in: path
        name: project
        description: The name of the cloud project that subscriptions belong to
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{project}/topics:
    get:
      summary: List Matching Topics
      description: Lists matching topics.
      operationId: pubsub.projects.topics.list
      x-api-path-slug: v1projecttopics-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of topics to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListTopicsResponse`; indicates
          that this isa continuation of a prior `ListTopics` call, and that the system
          shouldreturn the next page of data
      - in: path
        name: project
        description: The name of the cloud project that topics belong to
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{resource}:getIamPolicy:
    get:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for a resource.
        Returns an empty policy if the resource exists and does not have a policy
        set.
      operationId: pubsub.projects.topics.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-get
      parameters:
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
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