---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Contacts Get Public List
  description: Get the contact list for a user.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.contacts.getPublicList:
    get:
      summary: Contacts Get Public List
      description: Get the contact list for a user.
      operationId: getRestMethodFlickr.contacts.getpubliclist
      x-api-path-slug: restmethodflickr-contacts-getpubliclist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: user_id
        description: The NSID of the user to fetch the contact list for
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - GetPublicList
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