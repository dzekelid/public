---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 1
info:
  title: Victor Ops
  description: this-api-allows-you-to-interact-with-the-victorops-platform-in-various-ways--your-account-may-be-limitedto-a-total-number-of-api-calls-per-month--also-some-of-these-api-calls-have-rate-limits-note-in-this-documentation-when-creating-a-sample-curl-request-clicking-the-try-it-out-button-in-some-apiviewing-interfaces-the--in-an-email-address-may-be-encoded--please-note-that-the-rest-endpoints-will-notprocess-the-encoded-version--make-sure-that-the-encoded-character-40-is-changed-to-its-unencoded-form-beforesubmitting-the-curl-request-
  version: 0.0.2
host: api.victorops.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api-public/v2/team/{team}/oncall/schedule:
    get:
      summary: Get a team's on-call schedule
      description: |-
        Get the on-call schedule for a team, including on-call overrides.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v2.team.team.oncall.schedule.get
      x-api-path-slug: apipublicv2teamteamoncallschedule-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: team
        description: The VictorOps team slug
      responses:
        200:
          description: OK
      tags:
      - Api-public
      - V2
      - Team
      - Team
      - Oncall
      - Schedule
  /api-public/v2/user/{user}/oncall/schedule:
    get:
      summary: Get a user's on-call schedule
      description: |-
        Get the on-call schedule for a user for all teams the user is on, including on-call overrides.

        This API may be called a maximum of 15 times per minute.
      operationId: api_public.v2.user.user.oncall.schedule.get
      x-api-path-slug: apipublicv2useruseroncallschedule-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: user
        description: The VictorOps user ID
      responses:
        200:
          description: OK
      tags:
      - Api-public
      - V2
      - User
      - User
      - Oncall
      - Schedule
---