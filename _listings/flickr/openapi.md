---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
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
  /rest/?method=flickr.favorites.getPublicList:
    get:
      summary: Favorites Get Public List
      description: Returns a list of favorite public photos for the given user.
      operationId: getRestMethodFlickr.favorites.getpubliclist
      x-api-path-slug: restmethodflickr-favorites-getpubliclist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: max_fave_date
        description: Maximum date that a photo was favorited on
      - in: query
        name: min_fave_date
        description: Minimum date that a photo was favorited on
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: user_id
        description: The user to fetch the favorites list for
      responses:
        200:
          description: OK
      tags:
      - Favorites
      - GetPublicList
  /rest/?method=flickr.people.getPublicGroups:
    get:
      summary: People Get Public Groups
      description: Returns the list of public groups a user is a member of.
      operationId: getRestMethodFlickr.people.getpublicgroups
      x-api-path-slug: restmethodflickr-people-getpublicgroups-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: user_id
        description: The NSID of the user to fetch groups for
      responses:
        200:
          description: OK
      tags:
      - People
      - GetPublicGroups
  /rest/?method=flickr.people.getPublicPhotos:
    get:
      summary: People Get Public Photos
      description: Get a list of public photos for the given user.
      operationId: getRestMethodFlickr.people.getpublicphotos
      x-api-path-slug: restmethodflickr-people-getpublicphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
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
        name: safe_search
        description: Safe search setting
      - in: query
        name: user_id
        description: The NSID of the user whose photos to return
      responses:
        200:
          description: OK
      tags:
      - People
      - GetPublicPhotos
  /rest/?method=flickr.photos.getContactsPublicPhotos:
    get:
      summary: Photos Get Contacts Public Photos
      description: Fetch a list of recent public photos from a users' contacts.
      operationId: getRestMethodFlickr.photos.getcontactspublicphotos
      x-api-path-slug: restmethodflickr-photos-getcontactspublicphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: count
        description: Number of photos to return
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: include_self
        description: Set to 1 to include photos from the calling user
      - in: query
        name: just_friends
        description: Set as 1 to only show photos from friends and family (excluding
          regular contacts)
      - in: query
        name: single_photo
        description: Only fetch one photo (the latest) per contact, instead of all
          photos in chronological order
      - in: query
        name: user_id
        description: The NSID of the user to fetch photos for
      responses:
        200:
          description: OK
      tags:
      - Photos
      - GetContactsPublicPhotos
  /rest/?method=flickr.places.getChildrenWithPhotosPublic:
    get:
      summary: Places Get Children With Photos Public
      description: Return a list of locations with public photos that are parented
        by a Where on Earth (WOE) or Places ID.
      operationId: getRestMethodFlickr.places.getchildrenwithphotospublic
      x-api-path-slug: restmethodflickr-places-getchildrenwithphotospublic-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetChildrenWithPhotosPublic
---