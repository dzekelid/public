---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
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
  /?Action=UpdateSSHPublicKey:
    get:
      summary: Update S S H Public Key
      description: Sets the status of an IAM user's SSH public key to active or inactive.
      operationId: updateSSHPublicKey
      x-api-path-slug: actionupdatesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: Status
        description: The status to assign to the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
  /?Action=UploadSSHPublicKey:
    get:
      summary: Upload S S H Public Key
      description: Uploads an SSH public key and associates it with the specified
        IAM user.
      operationId: uploadSSHPublicKey
      x-api-path-slug: actionuploadsshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyBody
        description: The SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to associate the SSH public key with
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
---