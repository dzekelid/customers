---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Get Customer
  description: ""
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /customers?stateCode={stateCode}&countryCode={countryCode}&tagId={tagId}&marketplaceId={marketplaceId}&sortBy={sortBy}&sortDir={sortDir}&page={page}&pageSize={pageSize}
  : get:
      summary: List Customers
      description: Obtains a list of customers that match the specified criteria.
      operationId: customers_stateCode_stateCode_countryCode_countryCode_tagId_tagId_marketplaceId_marketplaceId_sortBy
      x-api-path-slug: customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get
      parameters:
      - in: path
        name: countryCode
        description: Returns customers that reside in the specified countryCode
      - in: path
        name: marketplaceId
        description: Returns customers that purchased items from the specified marketplaceId
      - in: path
        name: page
        description: Page number
      - in: path
        name: pageSize
        description: Requested page size
      - in: path
        name: sortBy
        description: Sorts the order of the response based off the specified value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: stateCode
        description: Returns customers that reside in the specified stateCode
      - in: path
        name: tagId
        description: Returns customers that have been tagged with the specified tagId
      responses:
        200:
          description: OK
      tags:
      - List
      - Customers
  /customers/{customerId}:
    get:
      summary: Get Customer
      description: ""
      operationId: customers.customerId.get
      x-api-path-slug: customerscustomerid-get
      parameters:
      - in: path
        name: customerId
        description: The system generated identifier for the Customer
      responses:
        200:
          description: OK
      tags:
      - Customer
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