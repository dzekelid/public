---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: Public
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops Get a team's on-call schedule
  x-api-slug: victor-ops
  description: |-
    Get the on-call schedule for a team, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v2/team/{team}/oncall/schedule
  tags: Api-public,V2,Team,Team,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/apipublicv2teamteamoncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/apipublicv2teamteamoncallschedule-get-openapi.md
- name: Victor Ops Get a user's on-call schedule
  x-api-slug: victor-ops
  description: |-
    Get the on-call schedule for a user for all teams the user is on, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v2/user/{user}/oncall/schedule
  tags: Api-public,V2,User,User,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/apipublicv2useruseroncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/apipublicv2useruseroncallschedule-get-openapi.md
- name: Victor Ops
  x-api-slug: victor-ops
  description: VictorOps incident managament software gives DevOps observability,
    collaboration, & real-time alerting, to build, deploy, & operate software. Learn
    more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com//
  tags: Public
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/victorops/openapi.md
x-common:
- type: x-blog
  url: https://victorops.com/blog/
- type: x-blog-rss
  url: https://victorops.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/victorops
- type: x-email
  url: support@victorops.com
- type: x-email
  url: info@victorops.com
- type: x-email
  url: press@victorops.com
- type: x-email
  url: sales@victorops.com
- type: x-github
  url: https://github.com/victorops
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: http://victorops.com
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---