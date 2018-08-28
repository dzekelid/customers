---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Retrieve customers
  version: 1.0.0
  description: Get a list of customers.
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