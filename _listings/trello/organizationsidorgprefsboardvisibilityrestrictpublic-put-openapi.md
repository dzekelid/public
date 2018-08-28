---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Organizations Preferences Boardvisibilityrestrict Public
  description: Put organizations preferences boardvisibilityrestrict public.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/public:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Public
      description: Put organizations preferences boardvisibilityrestrict public.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictPublicByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictpublic-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Public
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