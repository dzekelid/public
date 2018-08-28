swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/snippets/public:
    get:
      summary: Get Snippets Public
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3SnippetsPublic
      x-api-path-slug: v3snippetspublic-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Public