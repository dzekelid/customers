---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get a Customer
  description: Get a customer.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/customers:
    get:
      summary: Get Customers List
      description: Get customers list.
      operationId: V2CustomersGet
      x-api-path-slug: v2customers-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Customers
      - List
    post:
      summary: Create a Customer
      description: Create a customer.
      operationId: V2CustomersPost
      x-api-path-slug: v2customers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Customer
  /v2/customers/{customerID}:
    get:
      summary: Get a Customer
      description: Get a customer.
      operationId: V2CustomersByCustomerIDGet
      x-api-path-slug: v2customerscustomerid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
        description: A customer token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
    put:
      summary: Update a Customer
      description: Update a customer.
      operationId: V2CustomersByCustomerIDPut
      x-api-path-slug: v2customerscustomerid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
    delete:
      summary: Delete a Customer
      description: Deletes a customer.
      operationId: V2CustomersByCustomerIDDelete
      x-api-path-slug: v2customerscustomerid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
  /v2/carts/123456/checkout:
    post:
      summary: Checkout using customer id
      description: |-
        Converts a cart to an incomplete order. The original cart will remain and can be modified and checked out again if required.

        The new order will be returned and `data.meta.payment_gateways` will contain an array of the available payment gateways for this order.
      operationId: V2Carts123456CheckoutPost2
      x-api-path-slug: v2carts123456checkout-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Checkout
      - Using
      - Customer
      - Id
  '/v2/customers/tokens ':
    post:
      summary: Generate a customer token
      description: Generate a customer token.
      operationId: V2CustomersTokensPost
      x-api-path-slug: v2customerstokens-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Generate
      - Customer
      - Token
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