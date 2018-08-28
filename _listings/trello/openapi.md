swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
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