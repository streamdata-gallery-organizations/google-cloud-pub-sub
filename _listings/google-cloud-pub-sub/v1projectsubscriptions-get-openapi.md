---
swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 0
info:
  title: Google Cloud Pub/Sub API List Matching Subscription
  description: Lists matching subscriptions.
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