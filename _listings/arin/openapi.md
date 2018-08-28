swagger: "2.0"
x-collection-name: ARIN
x-complete: 1
info:
  title: Reverse DNS API
  description: for-managing-reverse-dns-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: www.arin.net
basePath: /regrws/core/v1
paths:
  /customers:
    get:
      summary: Manage customers
      description: ""
      operationId: customers
      x-api-path-slug: customers-get
      parameters:
      - in: query
        name: handle
        description: the handle of the customer
        type: string
        format: string
      - in: query
        name: name
        description: the name of the customer
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Customers