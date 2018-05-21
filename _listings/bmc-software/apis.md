---
name: BMC Software
x-slug: bmc-software
description: TrueSight Pulse responds to fluid IT demands with SaaS-based monitoring
  for real-time visibility into web-scale application metrics helping DevOps teams
  detect and diagnose problems fast.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
x-kinRank: "8"
x-alexaRank: ""
tags: Actions
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software API Get all available action types
  x-api-slug: bmc-software-api
  description: Gets all known action types
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actions-get-openapi.md
- name: BMC Software API Get all installed actions
  x-api-slug: bmc-software-api
  description: Gets all actions that are installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalled-get-openapi.md
- name: BMC Software API Install action
  x-api-slug: bmc-software-api
  description: Installs an action
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalled-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalled-put-openapi.md
- name: BMC Software API Get details of an installed action
  x-api-slug: bmc-software-api
  description: Gets a single action definition
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionid-get-openapi.md
- name: BMC Software API Get all alarms using an action
  x-api-slug: bmc-software-api
  description: Get alarms that are using this action installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId/alarms
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionidalarms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionidalarms-get-openapi.md
- name: BMC Software API Uninstall action
  x-api-slug: bmc-software-api
  description: Uninstalls an action and remove it from the associated alarms(s).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/installed/:actionId
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsinstalledactionid-delete-openapi.md
- name: BMC Software API Get action
  x-api-slug: bmc-software-api
  description: Gets a single action type
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/actions/:action
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsaction-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/v1actionsaction-get-openapi.md
- name: BMC Software API Get Actions (Alerts) List
  x-api-slug: bmc-software-api
  description: Returns a list of actions (alerts) that have been generated for your
    account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: |-
    https:////
        /api/{version}/actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/apiversionactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/apiversionactions-get-openapi.md
- name: BMC Software API Create Action
  x-api-slug: bmc-software-api
  description: Create a new Action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actions-post-openapi.md
- name: BMC Software API Update Action
  x-api-slug: bmc-software-api
  description: Update an existing Action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///actions/{action_id}
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actionsaction-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actionsaction-id-put-openapi.md
- name: BMC Software API List Actions
  x-api-slug: bmc-software-api
  description: List of all Actions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///actions
  tags: Actions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/actions-get-openapi.md
- name: BMC Software API
  x-api-slug: bmc-software-api
  description: TrueSight Pulse responds to fluid IT demands with SaaS-based monitoring
    for real-time visibility into web-scale application metrics helping DevOps teams
    detect and diagnose problems fast.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Actions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/actions/master/_listings/bmc-software/openapi.md
x-common:
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-github
  url: https://github.com/bmcsoftware
- type: x-twitter
  url: https://twitter.com/bmcsoftware
- type: x-website
  url: http://www.bmc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---