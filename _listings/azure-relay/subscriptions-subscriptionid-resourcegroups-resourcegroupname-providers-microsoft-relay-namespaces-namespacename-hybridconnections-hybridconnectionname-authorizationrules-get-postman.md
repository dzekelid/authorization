{
  "info": {
    "name": "Azure Relay API Hybrid Connections List Authorization Rules",
    "_postman_id": "5c135635-1d70-4003-b559-4b053938f7bc",
    "description": "Authorization rules for a HybridConnection.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hybrid connections authorization rules",
      "item": [
        {
          "id": "19924ec9-0f7a-498d-bdd9-a96f49a5ab3a",
          "name": "HybridConnections_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/HybridConnections/:hybridConnectionName/authorizationRules"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authorization rules for a HybridConnection"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8745d4a7-ea49-4f90-a099-90b25647a380"
            }
          ]
        }
      ]
    }
  ]
}