---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets get a filestream of vcard from customer
  description: Get a filestream of vcard from customer.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/vcard:
    get:
      summary: get a filestream of vcard from customer
      description: Get a filestream of vcard from customer.
      operationId: getRestAccountsContactsContactVcard
      x-api-path-slug: restaccountscontactscontactidvcard-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Get
      - Filestream
      - Of
      - Vcard
      - From
      - Customer
  /rest/items/sales_prices/{id}/customer_classes:
    get:
      summary: List activated customer classes
      description: Lists the activated customer classes for a sales price. The ID
        of the sales price must be specified.
      operationId: getRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Customer
      - Classes
    post:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: postRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/customer_classes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
  /rest/items/sales_prices/{id}/customer_classes/{customerClassId}:
    delete:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: deleteRestItemsSalesPricesCustomerClassesCustomerclass
      x-api-path-slug: restitemssales-pricesidcustomer-classescustomerclassid-delete
      parameters:
      - in: path
        name: customerClassId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
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