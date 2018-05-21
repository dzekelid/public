---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  description: github-is-the-best-place-to-share-code-with-friends-coworkers-classmates-and-complete-strangers-over-24-million-people-use-github-to-build-amazing-things-together-across-67-million-repositories-with-the-collaborative-features-of-githubcom-and-github-business-it-has-never-been-easier-for-individuals-and-teams-to-write-faster-better-code
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gists/public:
    get:
      summary: Get Gists Public
      description: List all public gists.
      operationId: list-all-public-gists
      x-api-path-slug: gistspublic-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: query
        name: since
        description: Timestamp in ISO 8601 format YYYY-MM-DDTHH:MM:SSZ
      responses:
        200:
          description: OK
      tags:
      - Gists
      - Public
  /orgs/{org}/public_members:
    get:
      summary: Get Orgs Org Public Members
      description: |-
        Public members list.
        Members of an organization can choose to have their membership publicized
        or not.
      operationId: public-members-listmembers-of-an-organization-can-choose-to-have-their-membership-publicizedor-not
      x-api-path-slug: orgsorgpublic-members-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Public
      - Members
  /orgs/{org}/public_members/{username}:
    delete:
      summary: Delete Orgs Org Public Members Username
      description: Conceal a user's membership.
      operationId: conceal-a-users-membership
      x-api-path-slug: orgsorgpublic-membersusername-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      - in: path
        name: username
        description: Name of the user
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Public
      - Members
      - Username
    get:
      summary: Get Orgs Org Public Members Username
      description: Check public membership.
      operationId: check-public-membership
      x-api-path-slug: orgsorgpublic-membersusername-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      - in: path
        name: username
        description: Name of the user
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Public
      - Members
      - Username
    put:
      summary: Put Orgs Org Public Members Username
      description: Publicize a user's membership.
      operationId: publicize-a-users-membership
      x-api-path-slug: orgsorgpublic-membersusername-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      - in: path
        name: username
        description: Name of the user
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Public
      - Members
      - Username
  /users/{username}/received_events/public:
    get:
      summary: Get Users Username Received Events Public
      description: List public events that a user has received
      operationId: list-public-events-that-a-user-has-received
      x-api-path-slug: usersusernamereceived-eventspublic-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Received
      - Events
      - Public
---