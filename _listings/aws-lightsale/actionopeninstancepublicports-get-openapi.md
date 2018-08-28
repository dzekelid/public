---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Open Instance Public Ports
  version: 1.0.0
  description: Adds public ports to an Amazon Lightsail instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CloseInstancePublicPorts:
    get:
      summary: Close Instance Public Ports
      description: Closes the public ports on a specific Amazon Lightsail instance.
      operationId: closeInstancePublicPorts
      x-api-path-slug: actioncloseinstancepublicports-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance on which youre attempting to close the
          public      ports
        type: string
      - in: query
        name: portInfo
        description: Information about the public port you are trying to close
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=OpenInstancePublicPorts:
    get:
      summary: Open Instance Public Ports
      description: Adds public ports to an Amazon Lightsail instance.
      operationId: openInstancePublicPorts
      x-api-path-slug: actionopeninstancepublicports-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance for which you want to open the public
          ports
        type: string
      - in: query
        name: portInfo
        description: An array of key-value pairs containing information about the
          port mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
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