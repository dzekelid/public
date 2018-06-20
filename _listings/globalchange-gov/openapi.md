---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
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
  /publication/{publication_identifier}:
    get:
      summary: Redirect to a particular publication.
      description: Given a numeric ID, redirect to the full URI of a publication.
      operationId: given-a-numeric-id-redirect-to-the-full-uri-of-a-publication
      x-api-path-slug: publicationpublication-identifier-get
      parameters:
      - in: path
        name: publication_identifier
        description: publication_identifier description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Particular
      - Publication
---