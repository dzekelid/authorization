{
  "info": {
    "name": "Azure Relay API Namespaces List Authorization Rules",
    "_postman_id": "fcd4813e-38d7-4d13-ac68-8d9dbb25757b",
    "description": "Authorization rules for a namespace.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces authorization rules",
      "item": [
        {
          "id": "c9e03d53-0b34-4c4b-88ca-3bfdf9e7c93d",
          "name": "Namespaces_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/AuthorizationRules"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authorization rules for a namespace"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d17f4266-c7b7-4711-93e8-4c821e0bf346"
            }
          ]
        }
      ]
    }
  ]
}