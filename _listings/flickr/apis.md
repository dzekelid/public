---
name: Flickr
x-slug: flickr
description: Flickr (pronounced flicker) is an image hosting and video hosting website,
  and web services suite that was created by Ludicorp in 2004 and acquired by Yahoo
  in 2005. In addition to being a popular website for users to share and embed personal
  photographs, and effectively an online community, the service is widely used by
  photo researchers and by bloggers to host images that they embed in blogs and social
  media.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Public
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/apis.md
specificationVersion: "0.14"
apis:
- name: Flickr Contacts Get Public List
  x-api-slug: flickr
  description: Get the contact list for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.contacts.getPublicList
  tags: Contacts,GetPublicList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-contacts-getpubliclist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-contacts-getpubliclist-get-openapi.md
- name: Flickr Favorites Get Public List
  x-api-slug: flickr
  description: Returns a list of favorite public photos for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.favorites.getPublicList
  tags: Favorites,GetPublicList
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-favorites-getpubliclist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-favorites-getpubliclist-get-openapi.md
- name: Flickr People Get Public Groups
  x-api-slug: flickr
  description: Returns the list of public groups a user is a member of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPublicGroups
  tags: People,GetPublicGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-people-getpublicgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-people-getpublicgroups-get-openapi.md
- name: Flickr People Get Public Photos
  x-api-slug: flickr
  description: Get a list of public photos for the given user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.people.getPublicPhotos
  tags: People,GetPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-people-getpublicphotos-get-openapi.md
- name: Flickr Photos Get Contacts Public Photos
  x-api-slug: flickr
  description: Fetch a list of recent public photos from a users' contacts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.photos.getContactsPublicPhotos
  tags: Photos,GetContactsPublicPhotos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-photos-getcontactspublicphotos-get-openapi.md
- name: Flickr Places Get Children With Photos Public
  x-api-slug: flickr
  description: Return a list of locations with public photos that are parented by
    a Where on Earth (WOE) or Places ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services///rest/?method=flickr.places.getChildrenWithPhotosPublic
  tags: Places,GetChildrenWithPhotosPublic
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/restmethodflickr-places-getchildrenwithphotospublic-get-openapi.md
- name: Flickr
  x-api-slug: flickr
  description: The Flickr API consists of a set of callable methods, and some API
    endpoints.  To perform an action using the Flickr API, you need to select a calling
    convention, send a request to its endpoint specifying a method and some arguments,
    and will receive a formatted response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/flickr-logo.jpg
  humanURL: http://www.flickr.com/
  baseURL: https://api.flickr.com//services/
  tags: Public
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/flickr/openapi.md
x-common:
- type: x-authentication
  url: https://www.flickr.com/services/api/auth.oauth.html
- type: x-base
  url: https://api.flickr.com/services/
- type: x-developer
  url: https://www.flickr.com/services/api/
- type: x-getting-started
  url: https://www.flickr.com/services/developer/
- type: x-privacy
  url: https://info.yahoo.com/privacy/us/yahoo/flickr/details.html
- type: x-support
  url: https://help.yahoo.com/kb/flickr-for-desktop
- type: x-terms-of-service
  url: https://www.flickr.com/services/api/tos/
- type: x-twitter
  url: https://twitter.com/flickr
- type: x-website
  url: http://www.flickr.com/
- type: x-website
  url: http://flickr.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---