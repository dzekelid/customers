---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Updates the customer's production
    option
  description: "Updates the customer's production option.   \nThe login user must
    be from the customer."
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms/{collaborationRoomId}/productionData/original/requirement:
    put:
      summary: Updates the customer's production option
      description: "Updates the customer's production option.   \nThe login user must
        be from the customer."
      operationId: updates-the-customers-production-option---the-login-user-must-be-from-the-customer
      x-api-path-slug: collaborationroomscollaborationroomidproductiondataoriginalrequirement-put
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: ProductionDataRequirementRequest
        description: A request about a production option
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Customers
      - Production
      - Option
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