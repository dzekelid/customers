---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns a list of customer booking limits.
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
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
  /consumer/v1/customers/customfields:
    get:
      summary: Returns a list of customField objects
      description: "This end point returns your Customer custom field definitions.\r\n\r\nCustomer
        custom fields are different than Appointment custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit, where as
        Customer custom fields are stored with the customer profile. \r\n\r\nUse the
        key field, and type to determine how to update field values\r\nin POST /consumer/v1/customers
        and PUT /consumer/v1/customers/{id}"
      operationId: ConsumerV1CustomersCustomfieldsGet
      x-api-path-slug: consumerv1customerscustomfields-get
      parameters:
      - in: query
        name: leadQuestions
        description: A true/false indicator to filter on custom fields used for lead
          questions
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customfields
  /consumer/v1/customers/registrationfields:
    get:
      summary: Returns a list of lead questions
      description: "This end point returns your Customer Registration fields.\r\n\r\nCustomer
        custom fields are different than Appointment custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit, where as
        Customer custom fields are stored with the customer profile."
      operationId: ConsumerV1CustomersRegistrationfieldsGet
      x-api-path-slug: consumerv1customersregistrationfields-get
      parameters:
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Registrationfields
  /consumer/v1/customers/plans:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersPlansGet
      x-api-path-slug: consumerv1customersplans-get
      parameters:
      - in: query
        name: groupId
        description: Filter customers by group
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
      - Plans
  /consumer/v1/customers/plans/{id}:
    get:
      summary: Returns a customer object.
      description: "The result returned is a single customer object. An id is required
        to find the customer. Find customer id's using either the GET consumer/v1/customers
        end point,\r\nor the GET consumer/v1/appointments end point. A customer object
        is automatically created with the first booking if it doesn't already exist."
      operationId: ConsumerV1CustomersPlansByIdGet
      x-api-path-slug: consumerv1customersplansid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Plans
  /consumer/v1/customers/{id}/planlimits/{serviceId}/{resourceId}/{dateTimeTz}:
    get:
      summary: Returns a list of customer booking limits.
      description: "The result returned is list of limit rules as defined by the subscribed
        customer plan along with Booking Counts/Minutes\r\nThe results indicate the
        remaining bookings count / minutes. Use the results in your app to determine
        if the customer should continue booking.\r\nYou can enforce Limits in periods:
        Daily,Weekly,Monthly and for maximum total limits. Maximum total limits is
        based on six months prior to\r\nthe DateTimeTz and six months after the DateTimeTz.
        Daily, Weekly and Monthly limits are based on the calculated period relative
        to the\r\nsubscription plan start. Daily,Weekly and Monthly limits can be
        setup on a per interval basis e.g. to biweekly, or daily every 10 days.\r\nSee
        customer plans setup in the Portal for more information.\r\nAll parameters
        are required. If resourceId is not applicable for a non-resource calendar,
        pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
      operationId: ConsumerV1CustomersByIdPlanlimitsByServiceIdByResourceIdByDateTimeTzGet
      x-api-path-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
      parameters:
      - in: path
        name: dateTimeTz
        description: The DateTimeTz to check
      - in: path
        name: id
        description: The id of the customer object
      - in: path
        name: resourceId
        description: The id of the resource object
      - in: path
        name: serviceId
        description: The id of the service object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Planlimits
      - ServiceId
      - ResourceId
      - DateTimeTz
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