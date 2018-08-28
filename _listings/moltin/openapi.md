swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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