---
name: GlobalChange.gov
x-slug: globalchange-gov
description: The U.S. Global Change Research Program (USGCRP) was established by Presidential
  Initiative in 1989 and mandated by Congress in the Global Change Research Act (GCRA)
  of 1990 to &ldquo;assist the Nation and the world to understand, assess, predict,
  and respond to human-induced and natural processes of global change.&rdquo;
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Public
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/apis.md
specificationVersion: "0.14"
apis:
- name: Global Change Information System API List generic publications.
  x-api-slug: global-change-information-system-api
  description: List the generic publications, 20 per page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////generic
  tags: Generic,Publications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/generic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/generic-get-openapi.md
- name: Global Change Information System API Get a representation of a generic publication.
  x-api-slug: global-change-information-system-api
  description: Get JSON which represents the structure of a generic publication.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////generic/{generic_identifier}
  tags: Representation,Generic,Publication
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/genericgeneric-identifier-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/genericgeneric-identifier-get-openapi.md
- name: Global Change Information System API Redirect to a particular publication.
  x-api-slug: global-change-information-system-api
  description: Given a numeric ID, redirect to the full URI of a publication.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////publication/{publication_identifier}
  tags: Redirect,To,Particular,Publication
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/publicationpublication-identifier-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/publicationpublication-identifier-get-openapi.md
- name: Global Change Information System API
  x-api-slug: global-change-information-system-api
  description: The U.S. Global Change Research Program (USGCRP) was established by
    Presidential Initiative in 1989 and mandated by Congress in the Global Change
    Research Act (GCRA) of 1990 to &ldquo;assist the Nation and the world to understand,
    assess, predict, and respond to human-induced and natural processes of global
    change.&rdquo;
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: Public
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/globalchange-gov/openapi.md
x-common:
- type: x-developer
  url: http://data.globalchange.gov/
- type: x-website
  url: http://globalchange.gov/
- type: x-website
  url: http://globalchange.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---