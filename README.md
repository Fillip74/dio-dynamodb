# dio-dynamodb

## Esquema da tabela ultilizada

```
{
  "TableName": "Filmes",
  "KeySchema": [
    {
      "KeyType": "HASH",
      "AttributeName": "Titulo"
    },
    {
      "KeyType": "RANGE",
      "AttributeName": "Ano"
    }
  ],
  "AttributeDefinitions": [
    {
      "AttributeName": "Titulo",
      "AttributeType": "S"
    },
    {
      "AttributeName": "Ano",
      "AttributeType": "S"
    }
  ],
  "BillingMode": "PROVISIONED",
  "ProvisionedThroughput": {
    "ReadCapacityUnits": 10,
    "WriteCapacityUnits": 5
  }
}
```