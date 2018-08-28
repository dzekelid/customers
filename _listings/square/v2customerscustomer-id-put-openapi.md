---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API UpdateCustomer
  description: |-
    Updates the details of an existing customer.
    The ID of the customer may change if the customer has been merged into another customer.

    You cannot edit a customer's cards on file with this endpoint. To make changes
    to a card on file, you must delete the existing card on file with the
    [DeleteCustomerCard](#endpoint-deletecustomercard) endpoint, then create a new one with the
    [CreateCustomerCard](#endpoint-createcustomercard) endpoint.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/customers/{customer_id}:
    delete:
      summary: DeleteCustomer
      description: Deletes a customer from a business, along with any linked cards
        on file.
      operationId: DeleteCustomer
      x-api-path-slug: v2customerscustomer-id-delete
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: customer_id
        description: The ID of the customer to delete
      responses:
        200:
          description: OK
      tags:
      - Customer
    put:
      summary: UpdateCustomer
      description: |-
        Updates the details of an existing customer.
        The ID of the customer may change if the customer has been merged into another customer.

        You cannot edit a customer's cards on file with this endpoint. To make changes
        to a card on file, you must delete the existing card on file with the
        [DeleteCustomerCard](#endpoint-deletecustomercard) endpoint, then create a new one with the
        [CreateCustomerCard](#endpoint-createcustomercard) endpoint.
      operationId: UpdateCustomer
      x-api-path-slug: v2customerscustomer-id-put
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customer_id
        description: The ID of the customer to update
      responses:
        200:
          description: OK
      tags:
      - Customer
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