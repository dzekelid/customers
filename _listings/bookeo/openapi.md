swagger: "2.0"
x-collection-name: Bookeo
x-complete: 1
info:
  title: Bookeo
  version: 1.0.0
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
    delete:
      summary: Delete a customer
      description: |-
        Delete a customer.
         Please note it is not possible to delete customers that have bookings in the future, and that are not cancelled.
         If your application needs to delete a customer with future bookings, make sure to cancel all future bookings for that customer first.
      operationId: deleteCustomers
      x-api-path-slug: customersid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{id}/authenticate:
    get:
      summary: Check a customer's password
      description: |-
        The customer's email address is the "username" used by Bookeo to authenticate customers.
         So to authenticate a customer your application would typically use GET /customers to search for customers with a given email address, and then GET /customers/{id}/authenticate to authenticate.
         Remember that there may be duplicate customer records with the same email address, ex. due to duplicate importing or manual record creation.
      operationId: getCustomersAuthenticate
      x-api-path-slug: customersidauthenticate-get
      parameters:
      - in: path
        name: id
      - in: query
        name: password
        description: remember to use URL encoding
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Authenticate
  /customers/{id}/bookings:
    get:
      summary: Retrieve a customer's bookings
      description: Retrieve a customer's bookings.
      operationId: getCustomersBookings
      x-api-path-slug: customersidbookings-get
      parameters:
      - in: query
        name: beginDate
        description: if specified, only bookings on or after this date will be included
      - in: query
        name: endDate
        description: if specified, only bookings on or before this date will be included
      - in: query
        name: expandParticipants
        description: if true, full details of the participants are included (provided
          the application has read permission over the participant)
      - in: path
        name: id
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Bookings
  /customers/{id}/linkedpeople:
    get:
      summary: Get the people linked to a customer
      description: Get the people linked to a customer.
      operationId: getCustomersLinkedpeople
      x-api-path-slug: customersidlinkedpeople-get
      parameters:
      - in: path
        name: id
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Linkedpeople
  /bookings/{bookingNumber}/customer:
    get:
      summary: Retrieve the customer associated with a booking
      description: Retrieve the customer associated with a booking.
      operationId: getBookingsBookingnumberCustomer
      x-api-path-slug: bookingsbookingnumbercustomer-get
      parameters:
      - in: path
        name: bookingNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Customer