swagger: "2.0"
x-collection-name: AWS DynamoDB
x-complete: 1
info:
  title: AWS DynamoDB API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=Scan:
    get:
      summary: Scan
      description: |-
        The Scan operation returns one or more items and item attributes by accessing every
              item in a table or a secondary index.
      operationId: scan
      x-api-path-slug: actionscan-get
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'A Boolean value that determines the read consistency model during
          the scan:'
        type: string
      - in: query
        name: ExclusiveStartKey
        description: The primary key of the first item that this operation will evaluate
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: FilterExpression
        description: A string that contains conditions that DynamoDB applies after
          the Scan operation, but       before the data is returned to you
        type: string
      - in: query
        name: IndexName
        description: The name of a secondary index to scan
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to evaluate (not necessarily the
          number of matching items)
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the specified table or index
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ScanFilter
        description: This is a legacy parameter
        type: string
      - in: query
        name: Segment
        description: For a parallel Scan request, Segment identifies an individual
          segment to be      scanned by an application worker
        type: string
      - in: query
        name: Select
        description: The attributes to be returned in the            result
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested items; or, if
          you provide             IndexName, the name of the table to which that index
          belongs
        type: string
      - in: query
        name: TotalSegments
        description: For a parallel Scan request, TotalSegments represents the total
          number of      segments into which the Scan operation will be divided
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scan