---
swagger: "2.0"
x-collection-name: VictorOps
x-complete: 0
info:
  title: Victor Ops Get a user's on-call schedule
  description: |-
    Get the on-call schedule for a user for all teams the user is on, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
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