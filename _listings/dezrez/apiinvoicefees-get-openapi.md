---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get agent fees invoices earned
  version: 1.0.0
  description: Get agent fees invoices earned.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/fee/getall:
    get:
      summary: Get list of all fees stored
      description: Get list of all fees stored.
      operationId: Fee_GetFeesBypageSizeBypageNumber
      x-api-path-slug: apifeegetall-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Fees
      - Stored
  /api/invoice/fees:
    get:
      summary: Get agent fees invoices earned
      description: Get agent fees invoices earned.
      operationId: Invoice_GetAgentFeesEarned
      x-api-path-slug: apiinvoicefees-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Agent
      - Fees
      - Invoices
      - Earned
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