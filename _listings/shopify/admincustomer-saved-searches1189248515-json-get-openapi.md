---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get one customer saved search by ID
  description: Get one customer saved search by id.
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
    post:
      summary: Creating a new address for a customer
      description: Creating a new address for a customer.
      operationId: postAdminCustomers3989659651Addresses.json
      x-api-path-slug: admincustomers3989659651addresses-json-post
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
      - Creating
      - New
      - Addressa
      - Customer
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
  /admin/customers/count.json:
    get:
      summary: Get a count of all customers
      description: Get a count of all customers.
      operationId: getAdminCustomersCount.json
      x-api-path-slug: admincustomerscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Customers
  /admin/customers.json:
    get:
      summary: Retrieve all customers
      description: Retrieve all customers.
      operationId: getAdminCustomers.json
      x-api-path-slug: admincustomers-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Customers
    post:
      summary: Create a new customer record
      description: Create a new customer record.
      operationId: postAdminCustomers.json
      x-api-path-slug: admincustomers-json-post
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
      - New
      - Customer
      - Record
  /admin/customers/3989659651/addresses/5436816654.json:
    get:
      summary: Get a single customers address
      description: Get a single customers address.
      operationId: getAdminCustomers3989659651Addresses5436816654.json
      x-api-path-slug: admincustomers3989659651addresses5436816654-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Customers
      - Address
  /admin/orders.json:
    get:
      summary: Get all orders from a customer
      description: Get all orders from a customer.
      operationId: getAdminOrders.json
      x-api-path-slug: adminorders-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: customer_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Orders
      - From
      - Customer
    post:
      summary: Create a pending order with an existing customer
      description: Create a pending order with an existing customer.
      operationId: postAdminOrders.json
      x-api-path-slug: adminorders-json-post
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
      - Pending
      - Order
      - Existing
      - Customer
  /admin/customers/3989659651/addresses/5436816654/default.json:
    put:
      summary: assigning a new default address to a customer
      description: Assigning a new default address to a customer.
      operationId: putAdminCustomers3989659651Addresses5436816654Default.json
      x-api-path-slug: admincustomers3989659651addresses5436816654default-json-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Assigning
      - New
      - Default
      - Address
      - To
      - Customer
  /admin/customers/3989659651/addresses/set.json:
    put:
      summary: destroying multiple customer addresses
      description: Destroying multiple customer addresses.
      operationId: putAdminCustomers3989659651AddressesSet.json
      x-api-path-slug: admincustomers3989659651addressesset-json-put
      parameters:
      - in: query
        name: address_ids[]
      - in: header
        name: Content-Type
      - in: query
        name: operation
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Destroying
      - Multiple
      - Customer
      - Addresses
  /admin/customers/5438892686.json:
    put:
      summary: Add metafield to an existing customer
      description: Add metafield to an existing customer.
      operationId: putAdminCustomers5438892686.json
      x-api-path-slug: admincustomers5438892686-json-put
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
      - Metafield
      - To
      - Existing
      - Customer
    delete:
      summary: Remove an existing customer
      description: Remove an existing customer.
      operationId: deleteAdminCustomers5438892686.json
      x-api-path-slug: admincustomers5438892686-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Existing
      - Customer
  /admin/customer_saved_searches/count.json:
    get:
      summary: Get a count of all customer saved searches
      description: Get a count of all customer saved searches.
      operationId: getAdminCustomerSavedSearchesCount.json
      x-api-path-slug: admincustomer-saved-searchescount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Customer
      - Saved
      - Searches
  /admin/customer_saved_searches.json:
    get:
      summary: Get all customer saved searches for a shop
      description: Get all customer saved searches for a shop.
      operationId: getAdminCustomerSavedSearches.json
      x-api-path-slug: admincustomer-saved-searches-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customer
      - Saved
      - Searchesa
      - Shop
    post:
      summary: Create a new Customer Saved Search
      description: Create a new customer saved search.
      operationId: postAdminCustomerSavedSearches.json
      x-api-path-slug: admincustomer-saved-searches-json-post
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
      - New
      - Customer
      - Saved
      - Search
  /admin/customers/3989659651.json:
    get:
      summary: Get a single customer by ID
      description: Get a single customer by id.
      operationId: getAdminCustomers3989659651.json
      x-api-path-slug: admincustomers3989659651-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Customer
      - By
      - ID
  /admin/customer_saved_searches/2029905294.json:
    put:
      summary: Update an existing Customer Saved Search
      description: Update an existing customer saved search.
      operationId: putAdminCustomerSavedSearches2029905294.json
      x-api-path-slug: admincustomer-saved-searches2029905294-json-put
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
      - Existing
      - Customer
      - Saved
      - Search
    delete:
      summary: Delete an existing Customer Saved Search
      description: Delete an existing customer saved search.
      operationId: deleteAdminCustomerSavedSearches2029905294.json
      x-api-path-slug: admincustomer-saved-searches2029905294-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Customer
      - Saved
      - Search
  /admin/customer_saved_searches/1189248515.json:
    get:
      summary: Get one customer saved search by ID
      description: Get one customer saved search by id.
      operationId: getAdminCustomerSavedSearches1189248515.json
      x-api-path-slug: admincustomer-saved-searches1189248515-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customer
      - Saved
      - Search
      - By
      - ID
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