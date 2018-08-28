swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
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