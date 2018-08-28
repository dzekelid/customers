---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Create a customer
  version: 1.0.0
  description: Creates an customer for a merchant.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/customers.csv:
    get:
      summary: Get a list of customers
      description: Gives information for every customer of a merchant by default.
      operationId: DelegatedGetCustomers
      x-api-path-slug: v3merchantsmidcustomers-csv-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - Csv
  /v3/merchants/{mId}/customers:
    get:
      summary: Get a list of customers
      description: Gives information for every customer of a merchant by default.
      operationId: DelegatedGetCustomers
      x-api-path-slug: v3merchantsmidcustomers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
    post:
      summary: Create a customer
      description: Creates an customer for a merchant.
      operationId: DelegatedCreateCustomer
      x-api-path-slug: v3merchantsmidcustomers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
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