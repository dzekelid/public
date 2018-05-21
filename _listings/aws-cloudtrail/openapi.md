---
swagger: "2.0"
x-collection-name: AWS CloudTrail
x-complete: 1
info:
  title: AWS CloudTrail API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListPublicKeys:
    get:
      summary: List Public Keys
      description: Returns all public keys whose private keys were used to sign the
        digest files within the specified time range.
      operationId: ListPublicKeys
      x-api-path-slug: actionlistpublickeys-get
      parameters:
      - in: query
        name: EndTime
        description: Optionally specifies, in UTC, the end of the time range to look
          up public keys for CloudTrail digest files
        type: string
      - in: query
        name: NextToken
        description: Reserved for future use
        type: string
      - in: query
        name: StartTime
        description: Optionally specifies, in UTC, the start of the time range to
          look up public keys for CloudTrail digest files
        type: string
      responses:
        200:
          description: OK
      tags:
      - Public Keys
---