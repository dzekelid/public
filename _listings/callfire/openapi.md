---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/public/{key}.{extension}:
    get:
      summary: Download media by extension
      description: 'Download a media file. Available types of files: bmp, gif, jpg,
        m4a, mp3, mp4, png, wav. Content type in response depends on ''extension''
        parameter, e.g. image/jpeg, image/png, audio/mp3, etc'
      operationId: getMediaDataByKey
      x-api-path-slug: mediapublickeyextension-get
      parameters:
      - in: path
        name: extension
        description: 'Media file type, available types: bmp, gif, jpg, m4a, mp3, mp4,
          png, wav'
      - in: path
        name: key
        description: A hash-key of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - Public
      - Key.extension
---