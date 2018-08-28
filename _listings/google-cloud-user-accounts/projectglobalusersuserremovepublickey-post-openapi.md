---
swagger: "2.0"
x-collection-name: Google Cloud User Accounts
x-complete: 0
info:
  title: Google Cloud User Accounts API Remove Public Key
  description: Removes the specified public key from the user.
  contact:
    name: Google
    url: https://google.com
  version: vm_alpha
host: www.googleapis.com
basePath: /clouduseraccounts/vm_alpha/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/users/{user}/addPublicKey:
    post:
      summary: Add Public Key
      description: Adds a public key to the specified User resource with the data
        included in the request.
      operationId: clouduseraccounts.users.addPublicKey
      x-api-path-slug: projectglobalusersuseraddpublickey-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
  /{project}/global/users/{user}/removePublicKey:
    post:
      summary: Remove Public Key
      description: Removes the specified public key from the user.
      operationId: clouduseraccounts.users.removePublicKey
      x-api-path-slug: projectglobalusersuserremovepublickey-post
      parameters:
      - in: query
        name: fingerprint
        description: The fingerprint of the public key to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
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