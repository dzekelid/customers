---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Update an existing customer
  version: 1.0.0
  description: Update an existing customer.
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers:
    get:
      summary: Retrieve customers
      description: Get a list of customers.
      operationId: getCustomers
      x-api-path-slug: customers-get
      parameters:
      - in: query
        name: createdSince
        description: if present, only include customers created since the given time
      - in: query
        name: currentMembers
        description: if true, include customers that are current members
      - in: query
        name: currentNonMembers
        description: if true, include customers that are not current members
      - in: query
        name: itemsPerPage
        description: number of items per page
      - in: query
        name: pageNavigationToken
        description: if present, continues navigation after a previous call
      - in: query
        name: pageNumber
      - in: query
        name: searchField
        description: a field on which to apply the search filter
      - in: query
        name: searchText
        description: the text to search for
      responses:
        200:
          description: OK
      tags:
      - Customers
    post:
      summary: Create a new customer.
      description: |-
        Create a new customer.
         Please note there is a limit to the number of customers that can be imported in Bookeo. Bookeo is primarily a booking system, not a CRM.
      operationId: postCustomers
      x-api-path-slug: customers-post
      parameters:
      - in: body
        name: customer
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{customerid}/linkedpeople/{id}:
    get:
      summary: Retrieve a person linked to a customer
      description: Retrieve a person linked to a customer.
      operationId: getCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-get
      parameters:
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
    put:
      summary: Update the details of a person linked to a customer
      description: Update the details of a person linked to a customer.
      operationId: putCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-put
      parameters:
      - in: body
        name: apiLinkedPerson
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
    delete:
      summary: Delete a person linked to a customer
      description: Delete a person linked to a customer.
      operationId: deleteCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-delete
      parameters:
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
  /customers/{id}:
    get:
      summary: Retrieve a customer
      description: Retrieve a customer by its id
      operationId: getCustomers
      x-api-path-slug: customersid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: Update an existing customer
      description: Update an existing customer.
      operationId: putCustomers
      x-api-path-slug: customersid-put
      parameters:
      - in: body
        name: customer
        schema:
          $ref: '#/definitions/holder'
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