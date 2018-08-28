---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Update a customer
  version: 1.0.0
  description: Updates information for a single customer. Only specified fields are
    overwritten.
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
  /v3/merchants/{mId}/customers/{customerId}:
    get:
      summary: Get a single customer
      description: Returns information for a single customer.
      operationId: DelegatedGetCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-get
      parameters:
      - in: path
        name: customerId
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
      - CustomerId
    post:
      summary: Update a customer
      description: Updates information for a single customer. Only specified fields
        are overwritten.
      operationId: DelegatedUpdateCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
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
      - CustomerId
    delete:
      summary: Delete a customer
      description: Deletes a single customer from a merchant.
      operationId: DelegatedDeleteCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
  /v3/merchants/{mId}/customers/{customerId}/phone_numbers:
    post:
      summary: Create a phone number for a customer
      description: Creates a phone number associated to a merchant's customer.
      operationId: DelegatedCreateCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
  /v3/merchants/{mId}/customers/{customerId}/phone_numbers/{phoneId}:
    post:
      summary: Update a phone number for a customer
      description: Updates a merchant's customer's phone number.
      operationId: DelegatedUpdateCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbersphoneid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: phoneId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
      - PhoneId
    delete:
      summary: Delete a customer phone number
      description: Deletes a merchant's customer's phone number.
      operationId: DelegatedDeleteCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbersphoneid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: phoneId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
      - PhoneId
  /v3/merchants/{mId}/customers/{customerId}/email_addresses:
    post:
      summary: Create an email address for a customer
      description: Creates an email address associated to a merchant's customer.
      operationId: DelegatedCreateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
  /v3/merchants/{mId}/customers/{customerId}/email_addresses/{emailId}:
    post:
      summary: Update an email address for a customer
      description: Updates a merchant's customer's email address.
      operationId: DelegatedUpdateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId
    delete:
      summary: Delete a customer email address
      description: Deletes a merchant's customer's email address.
      operationId: DelegatedDeleteCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId
  /v3/merchants/{mId}/customers/{customerId}/addresses:
    post:
      summary: Create an address for a customer
      description: Creates an address associated to a merchant's customer.
      operationId: DelegatedCreateCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
  /v3/merchants/{mId}/customers/{customerId}/addresses/{addressId}:
    post:
      summary: Update an address for a customer
      description: Updates a merchant's customer's address.
      operationId: DelegatedUpdateCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddressesaddressid-post
      parameters:
      - in: path
        name: addressId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
      - AddressId
    delete:
      summary: Delete a customer address
      description: Deletes a merchant's customer's address.
      operationId: DelegatedDeleteCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
      - AddressId
  /v3/merchants/{mId}/customers/{customerId}/cards:
    post:
      summary: Create a credit/debit card entry for a customer
      description: Create a credit/debit card entry for a customer.
      operationId: DelegatedCreateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcards-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
  /v3/merchants/{mId}/customers/{customerId}/cards/{cardId}:
    post:
      summary: Update a credit/debit card record for a customer
      description: Update a credit/debit card record for a customer.
      operationId: DelegatedUpdateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
    delete:
      summary: Delete a customer card
      description: Delete a customer card.
      operationId: DelegatedDeleteCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-delete
      parameters:
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
  /v3/merchants/{mId}/customers/{customerId}/metadata:
    post:
      summary: Create note, birthday, business name for a customer
      description: Creates note, birthday, business name associated to a merchant's
        customer.
      operationId: DelegatedCreateOrUpdateCustomerMetadata
      x-api-path-slug: v3merchantsmidcustomerscustomeridmetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Metadata
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