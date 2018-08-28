---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 0
info:
  title: AWS Service Catalog API Scan Provisioned Products
  version: 1.0.0
  description: |-
    Returns a paginated list of all the ProvisionedProduct objects that are currently
             available (not terminated).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ScanProvisionedProducts:
    get:
      summary: Scan Provisioned Products
      description: |-
        Returns a paginated list of all the ProvisionedProduct objects that are currently
                 available (not terminated).
      operationId: scanProvisionedProducts
      x-api-path-slug: actionscanprovisionedproducts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccessLevelFilter
        description: The access level for obtaining results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products
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