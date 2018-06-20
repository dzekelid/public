---
swagger: "2.0"
x-collection-name: Google Cloud User Accounts
x-complete: 1
info:
  title: Cloud User Accounts
  description: creates-and-manages-users-and-groups-for-accessing-google-compute-engine-virtual-machines-
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
  /{project}/zones/{zone}/authorizedKeysView/{user}:
    post:
      summary: Get Public Keys
      description: Returns a list of authorized public keys for a specific user account.
      operationId: clouduseraccounts.linux.getAuthorizedKeysView
      x-api-path-slug: projectzoneszoneauthorizedkeysviewuser-post
      parameters:
      - in: query
        name: instance
        description: The fully-qualified URL of the virtual machine requesting the
          view
      - in: query
        name: login
        description: Whether the view was requested as part of a user-initiated login
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: The user account for which you want to get a list of authorized
          public keys
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
  /{project}/zones/{zone}/linuxAccountViews:
    post:
      summary: Get Linux Account Views
      description: Retrieves a list of user accounts for an instance within a specific
        project.
      operationId: clouduseraccounts.linux.getLinuxAccountViews
      x-api-path-slug: projectzoneszonelinuxaccountviews-post
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: instance
        description: The fully-qualified URL of the virtual machine requesting the
          views
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
---