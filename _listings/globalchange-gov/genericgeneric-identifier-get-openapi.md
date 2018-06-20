---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get a representation of a generic publication.
  description: Get JSON which represents the structure of a generic publication.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /generic:
    get:
      summary: List generic publications.
      description: List the generic publications, 20 per page.
      operationId: list-the-generic-publications-20-per-page
      x-api-path-slug: generic-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the generic publications
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Generic
      - Publications
  /generic/{generic_identifier}:
    get:
      summary: Get a representation of a generic publication.
      description: Get JSON which represents the structure of a generic publication.
      operationId: get-json-which-represents-the-structure-of-a-generic-publication
      x-api-path-slug: genericgeneric-identifier-get
      parameters:
      - in: path
        name: generic_identifier
        description: generic_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Generic
      - Publication
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