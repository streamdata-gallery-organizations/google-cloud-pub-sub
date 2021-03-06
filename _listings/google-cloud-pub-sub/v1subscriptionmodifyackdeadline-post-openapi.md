---
swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 0
info:
  title: Google Cloud Pub/Sub API Modify ACK Deadline
  description: |-
    Modifies the ack deadline for a specific message. This method is useful
    to indicate that more time is needed to process a message by the
    subscriber, or to make the message available for redelivery if the
    processing was interrupted. Note that this does not modify the
    subscription-level `ackDeadlineSeconds` used for subsequent messages.
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
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on the specified resource. Replaces any
        existing policy.
      operationId: pubsub.projects.topics.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test IAM Permission
      description: |-
        Returns permissions that a caller has on the specified resource.
        If the resource does not exist, this will return an empty set of
        permissions, not a NOT_FOUND error.

        Note: This operation is designed to be used for building permission-aware
        UIs and command-line tools, not for authorization checking. This operation
        may "fail open" without warning.
      operationId: pubsub.projects.topics.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy detail is being
          requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{subscription}:
    delete:
      summary: Delete Subscription
      description: |-
        Deletes an existing subscription. All messages retained in the subscription
        are immediately dropped. Calls to `Pull` after deletion will return
        `NOT_FOUND`. After a subscription is deleted, a new one may be created with
        the same name, but the new one has no association with the old
        subscription or its topic unless the same topic is specified.
      operationId: pubsub.projects.subscriptions.delete
      x-api-path-slug: v1subscription-delete
      parameters:
      - in: path
        name: subscription
        description: The subscription to delete
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get Subscription
      description: Gets the configuration details of a subscription.
      operationId: pubsub.projects.subscriptions.get
      x-api-path-slug: v1subscription-get
      parameters:
      - in: path
        name: subscription
        description: The name of the subscription to get
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:acknowledge:
    post:
      summary: Acknowledge Subscription
      description: |-
        Acknowledges the messages associated with the `ack_ids` in the
        `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
        from the subscription.

        Acknowledging a message whose ack deadline has expired may succeed,
        but such a message may be redelivered later. Acknowledging a message more
        than once will not result in an error.
      operationId: pubsub.projects.subscriptions.acknowledge
      x-api-path-slug: v1subscriptionacknowledge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The subscription whose message is being acknowledged
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:modifyAckDeadline:
    post:
      summary: Modify ACK Deadline
      description: |-
        Modifies the ack deadline for a specific message. This method is useful
        to indicate that more time is needed to process a message by the
        subscriber, or to make the message available for redelivery if the
        processing was interrupted. Note that this does not modify the
        subscription-level `ackDeadlineSeconds` used for subsequent messages.
      operationId: pubsub.projects.subscriptions.modifyAckDeadline
      x-api-path-slug: v1subscriptionmodifyackdeadline-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The name of the subscription
      responses:
        200:
          description: OK
      tags:
      - ACK Deadline
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