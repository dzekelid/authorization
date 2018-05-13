{
  "info": {
    "name": "Azure Relay API Hybrid Connections Get Authorization Rule",
    "_postman_id": "ca3cda95-cfab-4ed4-9eb7-5c4f579bfe42",
    "description": "HybridConnection authorizationRule for a HybridConnection by name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hybrid connections authorization rule",
      "item": [
        {
          "id": "f4d905c9-dbd2-4a5d-b534-88a8d5b1a35f",
          "name": "HybridConnections_GetAuthorizationRule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/HybridConnections/:hybridConnectionName/authorizationRules/:authorizationRuleName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "namespaceName",
                  "value": "namespaceName",
                  "type": "string"
                },
                {
                  "id": "hybridConnectionName",
                  "value": "hybridConnectionName",
                  "type": "string"
                },
                {
                  "id": "authorizationRuleName",
                  "value": "authorizationRuleName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "HybridConnection authorizationRule for a HybridConnection by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9070d4-7312-4a85-b2b1-a835170e7029"
            }
          ]
        }
      ]
    }
  ]
}