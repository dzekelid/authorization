{
  "info": {
    "name": "Azure Relay API Hybrid Connections Delete Authorization Rule",
    "_postman_id": "6ee19cf7-a087-4280-8279-914005b9109f",
    "description": "Deletes a HybridConnection authorization rule",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "hybrid connections authorization rule",
      "item": [
        {
          "id": "b7bb3b43-d5d0-4e8f-9cae-b727a2e2f29f",
          "name": "HybridConnections_DeleteAuthorizationRule",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a HybridConnection authorization rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4e322cc-0a73-488d-8923-db0f5c5b7102"
            }
          ]
        }
      ]
    }
  ]
}