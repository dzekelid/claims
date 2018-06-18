---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting X-related-model Expenseclaims Expenseclaim
  description: X-related-model expenseclaims expenseclaim.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ExpenseClaims:
    get:
      summary: Get Expenseclaims
      description: Get expenseclaims.
      operationId: getExpenseclaims
      x-api-path-slug: expenseclaims-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
    post:
      summary: Post Expenseclaims
      description: Post expenseclaims.
      operationId: postExpenseclaims
      x-api-path-slug: expenseclaims-post
      parameters:
      - in: body
        name: ExpenseClaims
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
    put:
      summary: Put Expenseclaims
      description: Put expenseclaims.
      operationId: putExpenseclaims
      x-api-path-slug: expenseclaims-put
      parameters:
      - in: body
        name: ExpenseClaims
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
    x-related-model:
      summary: X-related-model Expenseclaims
      description: X-related-model expenseclaims.
      operationId: x-related-modelExpenseclaims
      x-api-path-slug: expenseclaims-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
  /ExpenseClaims/{ExpenseClaimID}:
    get:
      summary: Get Expenseclaims Expenseclaim
      description: Get expenseclaims expenseclaim.
      operationId: getExpenseclaimsExpenseclaim
      x-api-path-slug: expenseclaimsexpenseclaimid-get
      parameters:
      - in: path
        name: ExpenseClaimID
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
      - ExpenseClaimID
    post:
      summary: Post Expenseclaims Expenseclaim
      description: Post expenseclaims expenseclaim.
      operationId: postExpenseclaimsExpenseclaim
      x-api-path-slug: expenseclaimsexpenseclaimid-post
      parameters:
      - in: path
        name: ExpenseClaimID
      - in: body
        name: ExpenseClaims
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
      - ExpenseClaimID
    x-related-model:
      summary: X-related-model Expenseclaims Expenseclaim
      description: X-related-model expenseclaims expenseclaim.
      operationId: x-related-modelExpenseclaimsExpenseclaim
      x-api-path-slug: expenseclaimsexpenseclaimid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ExpenseClaims
      - ExpenseClaimID
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