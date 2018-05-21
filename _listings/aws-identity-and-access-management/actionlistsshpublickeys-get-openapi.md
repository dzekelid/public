---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API List S S H Public Keys
  version: 1.0.0
  description: Returns information about the SSH public keys associated with the specified
    IAM user.
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
  /?Action=GetSSHPublicKey:
    get:
      summary: Get S S H Public Key
      description: Retrieves the specified SSH public key, including metadata about
        the key.
      operationId: getSSHPublicKey
      x-api-path-slug: actiongetsshpublickey-get
      parameters:
      - in: query
        name: Encoding
        description: Specifies the public key encoding format to use in the response
        type: string
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
  /?Action=ListSSHPublicKeys:
    get:
      summary: List S S H Public Keys
      description: Returns information about the SSH public keys associated with the
        specified IAM user.
      operationId: listSSHPublicKeys
      x-api-path-slug: actionlistsshpublickeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to list SSH public keys for
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
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