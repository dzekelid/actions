---
name: EVRYTHNG
x-slug: evrythng
description: EVRYTHNG is the market leading internet of things platform for consumer
  product brands. Now individual product items can tell their stories to your business
  and your consumers throughout their lifecycle.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
x-kinRank: "7"
x-alexaRank: "686135"
tags: Actions
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/evrythng/apis.md
specificationVersion: "0.14"
apis:
- name: EVRYTHNG - /actions/scans (U)
  x-api-slug: actionsscans-post
  description: |-
    **USER** creates a "scan" action on a thng.

    **ATTENTION -->** use a valid thng ID in the payload!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/evrythng/actionsscans-post-openapi.md
- name: EVRYTHNG - /actions?project={id} (O)
  x-api-slug: actions-get
  description: '**OPERATOR** returns all the action types in the scope of an Application.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/evrythng/actions-get-openapi.md
- name: EVRYTHNG - /actions?project={id} (O)
  x-api-slug: actions-post
  description: '**OPERATOR** creates a new custom action type for app ID (visible
    only by that app).'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28871-evrythng-com.jpg
  humanURL: https://evrythng.com
  baseURL: https://example.com//
  tags: SaaS, Enterprise, Internet of Things, Profiles, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/evrythng/actions-post-openapi.md
x-common:
- type: x-deprecation
  url: https://developers.evrythng.com/docs/deprecation
- type: x-github
  url: https://github.com/evrythng
- type: x-postman-collection
  url: https://www.getpostman.com/collections/ba74e4cd196b0cffefec
- type: x-websub
  url: https://developers.evrythng.com/docs/pubsub
- type: x-api-gallery
  url: http://eventbrite.api.gallery.streamdata.io
- type: x-api-stack
  url: http://evrythng.stack.network
- type: x-authentication
  url: https://developers.evrythng.com/docs/authentication
- type: x-blog
  url: https://evrythng.com/blog/
- type: x-blog
  url: https://developers.evrythng.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/thngy
- type: x-email
  url: press@evrythng.com
- type: x-email
  url: privacy@evrythng.com
- type: x-security
  url: https://evrythng.com/securing-the-internet-of-things/
- type: x-support
  url: https://developers.evrythng.com/docs/support
- type: x-twitter
  url: https://twitter.com/EVRYTHNG
- type: x-website
  url: https://evrythng.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---