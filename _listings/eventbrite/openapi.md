---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: the-eventbrite-api-is-the-best-way-to-integrate-and-extend-eventbrite-for-your-event-or-organising-needs-version-3-of-the-api-brings-you-faster-responses-consistent-data-types-more-endpoints-and-easier-debugging-and-testing
  version: 1.0.0
host: www.eventbriteapi.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/public_discounts/:
    get:
      summary: Get Events  Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
    post:
      summary: Add Events  Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
  /events/{id}/public_discounts/:discount_id/:
    get:
      summary: Get Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
    post:
      summary: Add Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
    delete:
      summary: Delete Events  Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - ""
      - Public
      - Discounts
      - Discount
---