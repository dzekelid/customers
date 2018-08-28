---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Put Customer Attribute
  description: Put customer attribute.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customer:
    get:
      summary: Get Customer
      description: Get customer.
      operationId: getCustomer
      x-api-path-slug: customer-get
      parameters:
      - in: query
        name: email
        description: email
      responses:
        200:
          description: OK
      tags:
      - Customer
    post:
      summary: Post Customer
      description: Post customer.
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
    put:
      summary: Put Customer
      description: Put customer.
      operationId: putCustomer
      x-api-path-slug: customer-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
  /customer/address:
    get:
      summary: Get Customer Address
      description: Get customer address.
      operationId: getCustomerAddress
      x-api-path-slug: customeraddress-get
      parameters:
      - in: query
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
    put:
      summary: Put Customer Address
      description: Put customer address.
      operationId: putCustomerAddress
      x-api-path-slug: customeraddress-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
  /customer/address/{addressId}:
    put:
      summary: Put Customer Address Addressid
      description: Put customer address addressid.
      operationId: putCustomerAddressAddress
      x-api-path-slug: customeraddressaddressid-put
      parameters:
      - in: path
        name: addressId
        description: addressId
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressid
  /customer/address/{addressName}:
    delete:
      summary: Delete Customer Address Addressname
      description: Delete customer address addressname.
      operationId: deleteCustomerAddressAddressname
      x-api-path-slug: customeraddressaddressname-delete
      parameters:
      - in: path
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressname
  /customer/addresses:
    get:
      summary: Get Customer Addresses
      description: Get customer addresses.
      operationId: getCustomerAddresses
      x-api-path-slug: customeraddresses-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Resses
    delete:
      summary: Delete Customer Addresses
      description: Delete customer addresses.
      operationId: deleteCustomerAddresses
      x-api-path-slug: customeraddresses-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Resses
  /customer/attribute:
    put:
      summary: Put Customer Attribute
      description: Put customer attribute.
      operationId: putCustomerAttribute
      x-api-path-slug: customerattribute-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attribute
  /customer/attribute/{attributeName}:
    delete:
      summary: Delete Customer Attribute Attributename
      description: Delete customer attribute attributename.
      operationId: deleteCustomerAttributeAttributename
      x-api-path-slug: customerattributeattributename-delete
      parameters:
      - in: path
        name: attributeName
        description: attributeName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attribute
      - Attributename
  /customer/attributes:
    delete:
      summary: Delete Customer Attributes
      description: Delete customer attributes.
      operationId: deleteCustomerAttributes
      x-api-path-slug: customerattributes-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attributes
  /customer/password:
    post:
      summary: Post Customer Password
      description: Post customer password.
      operationId: postCustomerPassword
      x-api-path-slug: customerpassword-post
      parameters:
      - in: body
        name: changePasswordForm
        description: changePasswordForm
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Password
  /customer/payment:
    get:
      summary: Get Customer Payment
      description: Get customer payment.
      operationId: getCustomerPayment
      x-api-path-slug: customerpayment-get
      parameters:
      - in: query
        name: customerId
      - in: query
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
    post:
      summary: Post Customer Payment
      description: Post customer payment.
      operationId: postCustomerPayment
      x-api-path-slug: customerpayment-post
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
  /customer/payment/{paymentId}:
    put:
      summary: Put Customer Payment Paymentid
      description: Put customer payment paymentid.
      operationId: putCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-put
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
    delete:
      summary: Delete Customer Payment Paymentid
      description: Delete customer payment paymentid.
      operationId: deleteCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-delete
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
  /customer/payments:
    get:
      summary: Get Customer Payments
      description: Get customer payments.
      operationId: getCustomerPayments
      x-api-path-slug: customerpayments-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
    delete:
      summary: Delete Customer Payments
      description: Delete customer payments.
      operationId: deleteCustomerPayments
      x-api-path-slug: customerpayments-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
  /cart/checkout/payment/{customerPaymentId}:
    post:
      summary: Post Cart Checkout Payment Customerpaymentid
      description: Post cart checkout payment customerpaymentid.
      operationId: postCartCheckoutPaymentCustomerpayment
      x-api-path-slug: cartcheckoutpaymentcustomerpaymentid-post
      parameters:
      - in: query
        name: amount
        description: amount
      - in: query
        name: cartId
        description: cartId
      - in: query
        name: currency
        description: currency
      - in: path
        name: customerPaymentId
        description: customerPaymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Customerpaymentid
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