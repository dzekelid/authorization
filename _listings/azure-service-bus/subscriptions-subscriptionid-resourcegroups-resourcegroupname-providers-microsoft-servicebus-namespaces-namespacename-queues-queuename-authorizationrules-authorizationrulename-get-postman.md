{
  "info": {
    "name": "Azure Service Bus API Queues Get Authorization Rule",
    "_postman_id": "d4cce9b2-fe34-4e56-8365-43c3cb24fa8d",
    "description": "Gets an authorization rule for a queue by rule name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "queues authorization rule",
      "item": [
        {
          "id": "333b1340-4999-4814-abb1-e1eb2cc97ff9",
          "name": "Queues_GetAuthorizationRule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ServiceBus/namespaces/:namespaceName/queues/:queueName/authorizationRules/:authorizationRuleName"
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
                  "id": "queueName",
                  "value": "queueName",
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
            "description": "Gets an authorization rule for a queue by rule name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94ca3c6e-2f91-4814-aaae-7a6ba1b987bb"
            }
          ]
        }
      ]
    }
  ]
}