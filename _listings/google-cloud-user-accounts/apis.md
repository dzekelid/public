---
name: Google Cloud User Accounts
x-slug: google-cloud-user-accounts
description: Service for managing the global Google Cloud user accounts. This API
  reference is organized by resource type. Each resource type has one or more data
  representations and one or more methods.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Public
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud User Accounts API Add Public Key
  x-api-slug: google-cloud-user-accounts-api
  description: Adds a public key to the specified User resource with the data included
    in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
  baseURL: ://www.googleapis.com//clouduseraccounts/vm_alpha/projects//{project}/global/users/{user}/addPublicKey
  tags: Public Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/projectglobalusersuseraddpublickey-post-openapi.md
- name: Google Cloud User Accounts API Remove Public Key
  x-api-slug: google-cloud-user-accounts-api
  description: Removes the specified public key from the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
  baseURL: ://www.googleapis.com//clouduseraccounts/vm_alpha/projects//{project}/global/users/{user}/removePublicKey
  tags: Public Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/projectglobalusersuserremovepublickey-post-openapi.md
- name: Google Cloud User Accounts API Get Public Keys
  x-api-slug: google-cloud-user-accounts-api
  description: Returns a list of authorized public keys for a specific user account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
  baseURL: ://www.googleapis.com//clouduseraccounts/vm_alpha/projects//{project}/zones/{zone}/authorizedKeysView/{user}
  tags: Public Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/projectzoneszoneauthorizedkeysviewuser-post-openapi.md
- name: Google Cloud User Accounts API Get Linux Account Views
  x-api-slug: google-cloud-user-accounts-api
  description: Retrieves a list of user accounts for an instance within a specific
    project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
  baseURL: ://www.googleapis.com//clouduseraccounts/vm_alpha/projects//{project}/zones/{zone}/linuxAccountViews
  tags: Public Key
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/projectzoneszonelinuxaccountviews-post-openapi.md
- name: Google Cloud User Accounts API
  x-api-slug: google-cloud-user-accounts-api
  description: Service for managing the global Google Cloud user accounts. This API
    reference is organized by resource type. Each resource type has one or more data
    representations and one or more methods.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-icon.png
  humanURL: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
  baseURL: ://www.googleapis.com//clouduseraccounts/vm_alpha/projects
  tags: Public
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/public/master/_listings/google-cloud-user-accounts/openapi.md
x-common:
- type: x-code
  url: https://cloud.google.com/compute/docs/access/user-accounts/api/libraries
- type: x-guides
  url: https://cloud.google.com/compute/docs/access/user-accounts/api/how-tos/how-tos
- type: x-website
  url: https://cloud.google.com/compute/docs/access/user-accounts/api/latest/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---