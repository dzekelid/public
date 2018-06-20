---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 1
info:
  title: StorSimpleSeries8000ManagementClient
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/listPublicEncryptionKey
  : post:
      summary: Managers Get Public Encryption Key
      description: Returns the symmetric encrypted public encryption key of the manager.
      operationId: Managers_GetPublicEncryptionKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamelistpublicencryptionkey-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Managers Public Encryption Key
---