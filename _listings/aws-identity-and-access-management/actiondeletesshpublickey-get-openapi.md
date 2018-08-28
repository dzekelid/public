---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Delete S S H Public Key
  version: 1.0.0
  description: Deletes the specified SSH public key.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteSSHPublicKey:
    get:
      summary: Delete S S H Public Key
      description: Deletes the specified SSH public key.
      operationId: deleteSSHPublicKey
      x-api-path-slug: actiondeletesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
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