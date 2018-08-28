---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get all customers who match the criteria
  description: Get all customers who match the criteria.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customers/3989659651/addresses/5484465742.json:
    put:
      summary: Updating a customers postal code
      description: Updating a customers postal code.
      operationId: putAdminCustomers3989659651Addresses5484465742.json
      x-api-path-slug: admincustomers3989659651addresses5484465742-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Updating
      - Customers
      - Postal
      - Code
    delete:
      summary: Removing a customers address
      description: Removing a customers address.
      operationId: deleteAdminCustomers3989659651Addresses5484465742.json
      x-api-path-slug: admincustomers3989659651addresses5484465742-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Removing
      - Customers
      - Address
  /admin/customers/search.json:
    get:
      summary: Get all customers with an address in the Brazil
      description: Get all customers with an address in the brazil.
      operationId: getAdminCustomersSearch.json
      x-api-path-slug: admincustomerssearch-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Address
      - In
      - Brazil
  /admin/customers/3989659651/addresses.json:
    get:
      summary: Get all of a customer's addresses
      description: Get all of a customer's addresses.
      operationId: getAdminCustomers3989659651Addresses.json
      x-api-path-slug: admincustomers3989659651addresses-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Addresses
  /admin/customer_saved_searches/1189248515/customers.json:
    get:
      summary: Get all customers who match the criteria
      description: Get all customers who match the criteria.
      operationId: getAdminCustomerSavedSearches1189248515Customers.json
      x-api-path-slug: admincustomer-saved-searches1189248515customers-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Who
      - Match
      - Criteria
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