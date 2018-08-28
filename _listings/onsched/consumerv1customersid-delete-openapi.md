---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Deletes a customer subscription object.
  description: Deletes a customer subscription object.
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/customers:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersGet
      x-api-path-slug: consumerv1customers-get
      parameters:
      - in: query
        name: deleted
        description: Filter customers by deleted status
      - in: query
        name: email
        description: Filter customers by email address
      - in: query
        name: groupId
        description: Filter customers by group
      - in: query
        name: lastname
        description: Search customers by lastname
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
    post:
      summary: Creates a new customer object.
      description: "Use this endpoint to create a new customer. If not specified the
        business location id defaults to the first location in the company.\r\nEmail
        Address and a lastname are required for creating a new customer."
      operationId: ConsumerV1CustomersPost
      x-api-path-slug: consumerv1customers-post
      parameters:
      - in: body
        name: customerIM
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customers
  /consumer/v1/customers/{id}:
    get:
      summary: Returns a customer object.
      description: "The result returned is a single customer object. An id is required
        to find the customer. Find customer id's using either the GET consumer/v1/customers
        end point,\r\nor the GET consumer/v1/appointments end point. A customer object
        is automatically created with the first booking if it doesn't already exist."
      operationId: ConsumerV1CustomersByIdGet
      x-api-path-slug: consumerv1customersid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: Updates a customer object.
      description: "Use this endpoint to update customer information. If not specified
        the business location id defaults to the first location in the company.\r\nBlank
        fields are not changed"
      operationId: ConsumerV1CustomersByIdPut
      x-api-path-slug: consumerv1customersid-put
      parameters:
      - in: body
        name: customerUM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
    delete:
      summary: Deletes a customer subscription object.
      description: Deletes a customer subscription object.
      operationId: ConsumerV1CustomersByIdDelete
      x-api-path-slug: consumerv1customersid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
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