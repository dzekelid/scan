{
  "info": {
    "name": "Amazon DynamoDB API Scan",
    "_postman_id": "7e95fc01-ff1e-4ef0-9ea0-a36277ce197b",
    "description": "The Scan operation returns one or more items and item attributes by accessing every\n      item in a table or a secondary index.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Batch Items",
      "item": [
        {
          "id": "76c4481c-d667-4ed6-b9a8-3749f65f5903",
          "name": "batchGetItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchGetItem operation returns the attributes of one or more items from one or\n      more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d40b0abb-9e3c-40a4-b409-5ea3adfba71e"
            }
          ]
        },
        {
          "id": "b52ccb59-affe-447f-b233-7182abcbeb48",
          "name": "batchWriteItem",
          "request": {
            "url": "http://example.com/api/?Action=BatchWriteItem?RequestItems=RequestItems&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The BatchWriteItem operation puts or deletes multiple items in one or more tables."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0c57f7b-534d-4130-a85b-8a19f4bc2072"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "5ef0960b-936a-4ef7-9a36-842b17e0b311",
          "name": "createTable",
          "request": {
            "url": "http://example.com/api/?Action=CreateTable?AttributeDefinitions=AttributeDefinitions&GlobalSecondaryIndexes=GlobalSecondaryIndexes&KeySchema=KeySchema&LocalSecondaryIndexes=LocalSecondaryIndexes&ProvisionedThroughput=ProvisionedThroughput&StreamSpecification=StreamSpecification&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The CreateTable operation adds a new table to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3386e9e5-06ff-4238-899c-225e0b4bf8dc"
            }
          ]
        },
        {
          "id": "88e374e7-4d53-4ee9-a259-0a9e8910c7b6",
          "name": "deleteTable",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteTable operation deletes a table and all of its items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fb00b51-ccb1-4ccb-8201-ceb447608b48"
            }
          ]
        },
        {
          "id": "c482a5a6-3c5d-41aa-850d-4a8cc34e7c5c",
          "name": "describeTable",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTable?TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the table, including the current status of the table, when it was created, the primary key schema, and any indexes on the table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2c4975e-6fdd-4001-a656-15025b76f718"
            }
          ]
        },
        {
          "id": "f2ce12e5-7939-4a40-80cb-4a96e6cdfd88",
          "name": "listTables",
          "request": {
            "url": "http://example.com/api/?Action=ListTables?ExclusiveStartTableName=ExclusiveStartTableName&Limit=Limit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of table names associated with the current account and endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "013aff29-96aa-4374-8c44-f509b209d939"
            }
          ]
        }
      ]
    },
    {
      "name": "Items",
      "item": [
        {
          "id": "ee1d6c2d-15d4-494d-b2d0-a116a225baef",
          "name": "deleteItem",
          "request": {
            "url": "http://example.com/api/?Action=DeleteItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Key=Key&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a single item in a table by primary key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4d8904e-e2e6-4978-9d90-f313afbaef3d"
            }
          ]
        },
        {
          "id": "d9f74532-8d9d-4981-bb42-f8dcf5a70aaf",
          "name": "getItem",
          "request": {
            "url": "http://example.com/api/?Action=GetItem?AttributesToGet=AttributesToGet&ConsistentRead=ConsistentRead&ExpressionAttributeNames=ExpressionAttributeNames&Key=Key&ProjectionExpression=ProjectionExpression&ReturnConsumedCapacity=ReturnConsumedCapacity&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The GetItem operation returns a set of attributes for the item with the given primary\n          key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8ebe024-50c8-458c-9a59-5bc35086696a"
            }
          ]
        },
        {
          "id": "2b286860-a87b-4d1f-b032-f662303a0975",
          "name": "putItem",
          "request": {
            "url": "http://example.com/api/?Action=PutItem?ConditionalOperator=ConditionalOperator&ConditionExpression=ConditionExpression&Expected=Expected&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&Item=Item&ReturnConsumedCapacity=ReturnConsumedCapacity&ReturnItemCollectionMetrics=ReturnItemCollectionMetrics&ReturnValues=ReturnValues&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new item, or replaces an old item with a new item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7df50aa-8af4-4f3a-bd0b-9277f819ac57"
            }
          ]
        }
      ]
    },
    {
      "name": "Limits",
      "item": [
        {
          "id": "cd31883f-00c5-43b9-be55-92ffd2655467",
          "name": "describeLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLimits?AccountMaxReadCapacityUnits=AccountMaxReadCapacityUnits&AccountMaxWriteCapacityUnits=AccountMaxWriteCapacityUnits&TableMaxReadCapacityUnits=TableMaxReadCapacityUnits&TableMaxWriteCapacityUnits=TableMaxWriteCapacityUnits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current provisioned-capacity limits for your AWS account in a region, both for the region as a whole and for any one DynamoDB table that you create there."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd325fbc-6c23-46e0-b483-f33255f6136a"
            }
          ]
        }
      ]
    },
    {
      "name": "Query",
      "item": [
        {
          "id": "10915c5c-fbe2-4f58-81ef-80fffd3f7f4d",
          "name": "query",
          "request": {
            "url": "http://example.com/api/?Action=Query?AttributesToGet=AttributesToGet&ConditionalOperator=ConditionalOperator&ConsistentRead=ConsistentRead&ExclusiveStartKey=ExclusiveStartKey&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&FilterExpression=FilterExpression&IndexName=IndexName&KeyConditionExpression=KeyConditionExpression&KeyConditions=KeyConditions&Limit=Limit&ProjectionExpression=ProjectionExpression&QueryFilter=QueryFilter&ReturnConsumedCapacity=ReturnConsumedCapacity&ScanIndexForward=ScanIndexForward&Select=Select&TableName=TableName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A Query operation uses the primary key of a table or a secondary index\n            to directly access items from that table or index."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa628d7b-e8f7-467f-85ed-c16dcaf27f3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Scan",
      "item": [
        {
          "id": "da6b7db7-cae2-4613-91ad-647134b153f2",
          "name": "scan",
          "request": {
            "url": "http://example.com/api/?Action=Scan?AttributesToGet=AttributesToGet&ConditionalOperator=ConditionalOperator&ConsistentRead=ConsistentRead&ExclusiveStartKey=ExclusiveStartKey&ExpressionAttributeNames=ExpressionAttributeNames&ExpressionAttributeValues=ExpressionAttributeValues&FilterExpression=FilterExpression&IndexName=IndexName&Limit=Limit&ProjectionExpression=ProjectionExpression&ReturnConsumedCapacity=ReturnConsumedCapacity&ScanFilter=ScanFilter&Segment=Segment&Select=Select&TableName=TableName&TotalSegments=TotalSegments",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Scan operation returns one or more items and item attributes by accessing every\n      item in a table or a secondary index."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75a81a49-0ae3-49fb-9dbd-81471d83c449"
            }
          ]
        }
      ]
    }
  ]
}