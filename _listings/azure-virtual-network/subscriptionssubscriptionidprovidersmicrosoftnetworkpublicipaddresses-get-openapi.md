---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Public IPAddresses List All
  description: Gets all the public IP addresses in a subscription.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/publicIPAddresses/{publicIpAddressName}
  : delete:
      summary: Public IPAddresses Delete
      description: Deletes the specified public IP address.
      operationId: PublicIPAddresses_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkpublicipaddressespublicipaddressname-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: publicIpAddressName
        description: The name of the subnet
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Public IP Address
    get:
      summary: Public IPAddresses Get
      description: Gets the specified public IP address in a specified resource group.
      operationId: PublicIPAddresses_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkpublicipaddressespublicipaddressname-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced resources
      - in: query
        name: No Name
      - in: path
        name: publicIpAddressName
        description: The name of the subnet
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Public IP Address
    put:
      summary: Public IPAddresses Create Or Update
      description: Creates or updates a static or dynamic public IP address.
      operationId: PublicIPAddresses_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworkpublicipaddressespublicipaddressname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create or update public IP address
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: publicIpAddressName
        description: The name of the public IP address
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Public IP Address
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/publicIPAddresses:
    get:
      summary: Public IPAddresses List All
      description: Gets all the public IP addresses in a subscription.
      operationId: PublicIPAddresses_ListAll
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftnetworkpublicipaddresses-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Public IP Address
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