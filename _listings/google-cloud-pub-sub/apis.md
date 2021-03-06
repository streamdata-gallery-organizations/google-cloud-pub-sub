---
name: Google Cloud Pub Sub
x-slug: google-cloud-pub-sub
description: Cloud Pub/Sub is a fully-managed real-time messaging service that allows
  you to send and receive messages between independent applications. You can leverage
  Cloud Pub/Sub&rsquo;s flexibility to decouple systems and components hosted on Google
  Cloud Platform or elsewhere on the Internet. By building on the same technology
  Google uses, Cloud Pub/Sub is designed to provide &ldquo;at least once&rdquo; delivery
  at low latency with on-demand scalability to 1 million messages per second (and
  beyond).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Cloud Pub Sub
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Pub/Sub - Create Topic
  x-api-slug: v1name-put
  description: Creates the given topic with the given name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1name-put-openapi.md
- name: Google Cloud Pub/Sub - List Matching Subscription
  x-api-slug: v1projectsubscriptions-get
  description: Lists matching subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1projectsubscriptions-get-openapi.md
- name: Google Cloud Pub/Sub - List Matching Topics
  x-api-slug: v1projecttopics-get
  description: Lists matching topics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1projecttopics-get-openapi.md
- name: Google Cloud Pub/Sub - Get IAM Policy
  x-api-slug: v1resourcegetiampolicy-get
  description: |-
    Gets the access control policy for a resource.
    Returns an empty policy if the resource exists and does not have a policy
    set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1resourcegetiampolicy-get-openapi.md
- name: Google Cloud Pub/Sub - Set IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on the specified resource. Replaces any
    existing policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1resourcesetiampolicy-post-openapi.md
- name: Google Cloud Pub/Sub - Test IAM Permission
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified resource.
    If the resource does not exist, this will return an empty set of
    permissions, not a NOT_FOUND error.

    Note: This operation is designed to be used for building permission-aware
    UIs and command-line tools, not for authorization checking. This operation
    may "fail open" without warning.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1resourcetestiampermissions-post-openapi.md
- name: Google Cloud Pub/Sub - Delete Subscription
  x-api-slug: v1subscription-delete
  description: |-
    Deletes an existing subscription. All messages retained in the subscription
    are immediately dropped. Calls to `Pull` after deletion will return
    `NOT_FOUND`. After a subscription is deleted, a new one may be created with
    the same name, but the new one has no association with the old
    subscription or its topic unless the same topic is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscription-delete-openapi.md
- name: Google Cloud Pub/Sub - Get Subscription
  x-api-slug: v1subscription-get
  description: Gets the configuration details of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscription-get-openapi.md
- name: Google Cloud Pub/Sub - Acknowledge Subscription
  x-api-slug: v1subscriptionacknowledge-post
  description: |-
    Acknowledges the messages associated with the `ack_ids` in the
    `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
    from the subscription.

    Acknowledging a message whose ack deadline has expired may succeed,
    but such a message may be redelivered later. Acknowledging a message more
    than once will not result in an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscriptionacknowledge-post-openapi.md
- name: Google Cloud Pub/Sub - Modify ACK Deadline
  x-api-slug: v1subscriptionmodifyackdeadline-post
  description: |-
    Modifies the ack deadline for a specific message. This method is useful
    to indicate that more time is needed to process a message by the
    subscriber, or to make the message available for redelivery if the
    processing was interrupted. Note that this does not modify the
    subscription-level `ackDeadlineSeconds` used for subsequent messages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscriptionmodifyackdeadline-post-openapi.md
- name: Google Cloud Pub/Sub - Modify Push Configuration
  x-api-slug: v1subscriptionmodifypushconfig-post
  description: |-
    Modifies the `PushConfig` for a specified subscription.

    This may be used to change a push subscription to a pull one (signified by
    an empty `PushConfig`) or vice versa, or change the endpoint URL and other
    attributes of a push subscription. Messages will accumulate for delivery
    continuously through the call regardless of changes to the `PushConfig`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscriptionmodifypushconfig-post-openapi.md
- name: Google Cloud Pub/Sub - Pull Message
  x-api-slug: v1subscriptionpull-post
  description: |-
    Pulls messages from the server. Returns an empty list if there are no
    messages available in the backlog. The server may return `UNAVAILABLE` if
    there are too many concurrent pull requests pending for the given
    subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1subscriptionpull-post-openapi.md
- name: Google Cloud Pub/Sub - Delete Topic
  x-api-slug: v1topic-delete
  description: |-
    Deletes the topic with the given name. Returns `NOT_FOUND` if the topic
    does not exist. After a topic is deleted, a new topic may be created with
    the same name; this is an entirely new topic with none of the old
    configuration or subscriptions. Existing subscriptions to this topic are
    not deleted, but their `topic` field is set to `_deleted-topic_`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1topic-delete-openapi.md
- name: Google Cloud Pub/Sub - Get Topic Configuration
  x-api-slug: v1topic-get
  description: Gets the configuration of a topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1topic-get-openapi.md
- name: Google Cloud Pub/Sub - Get Topic Subscription
  x-api-slug: v1topicsubscriptions-get
  description: Lists the name of the subscriptions for this topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1topicsubscriptions-get-openapi.md
- name: Google Cloud Pub/Sub - Publish Topic
  x-api-slug: v1topicpublish-post
  description: |-
    Adds one or more messages to the topic. Returns `NOT_FOUND` if the topic
    does not exist. The message payload must not be empty; it must contain
     either a non-empty data field, or at least one attribute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-cloud-pub-sub/master/_listings/google-cloud-pub-sub/v1topicpublish-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.prediction.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.pub.sub.stack.network
- type: x-change-log
  url: https://cloud.google.com/pubsub/docs/release-notes
- type: x-code
  url: https://cloud.google.com/pubsub/docs/reference/libraries
- type: x-faq
  url: https://cloud.google.com/pubsub/docs/faq
- type: x-getting-started
  url: https://cloud.google.com/pubsub/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/pubsub/docs/how-to
- type: x-issues
  url: https://issuetracker.google.com/issues?q=componentid:187173%20status:open
- type: x-pricing
  url: https://cloud.google.com/pubsub/pricing
- type: x-rate-limits
  url: https://cloud.google.com/pubsub/quotas
- type: x-service-level-agreement
  url: https://cloud.google.com/pubsub/sla
- type: x-support
  url: https://cloud.google.com/pubsub/docs/support
- type: x-website
  url: https://cloud.google.com/pubsub/docs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---