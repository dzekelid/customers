---
swagger: "2.0"
x-collection-name: Intuit
x-complete: 0
info:
  title: QuickBooks Online V3 API Get Reports Customer Income
  description: |-
    Report - Customer Income
    Method : GET
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/CustomerBalanceDetail:
    get:
      summary: Get Reports Customer Balance Detail
      description: |-
        Report - CustomerBalance Detail
        Method : GET

        The information below provides a reference on how to access the Customer Balance Detail report from the QuickBooks Online Report Service.
      operationId: getReportsCustomerbalancedetail
      x-api-path-slug: reportscustomerbalancedetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
      - Detail
  /customer:
    post:
      summary: Post Customer
      description: |-
        Create a customer
        Method : POST
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Customer
  /customer/63:
    get:
      summary: Get Customer
      description: |-
        Read a customer entry by Id
        Method : GET
      operationId: getCustomer63
      x-api-path-slug: customer63-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Customer
  /reports/CustomerIncome:
    get:
      summary: Get Reports Customer Income
      description: |-
        Report - Customer Income
        Method : GET
      operationId: getReportsCustomerincome
      x-api-path-slug: reportscustomerincome-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Income
  /reports/CustomerBalance:
    get:
      summary: Get Reports Customer Balance
      description: |-
        Report - CustomerBalance
        Method : GET
      operationId: getReportsCustomerbalance
      x-api-path-slug: reportscustomerbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
  /reports/CustomerSales:
    get:
      summary: Get Reports Customer Sales
      description: |-
        Report - Customer Sales
        Method : GET
      operationId: getReportsCustomersales
      x-api-path-slug: reportscustomersales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Sales
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