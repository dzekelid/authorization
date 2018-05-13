{
  "info": {
    "name": "Azure Relay API Namespaces Get Authorization Rule",
    "_postman_id": "939aa800-cf96-4ec7-ad9f-07d759ddfba6",
    "description": "Authorization rule for a namespace by name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "namespaces authorization rule",
      "item": [
        {
          "id": "74f9833b-2583-42b4-bab1-54beebf02410",
          "name": "Namespaces_GetAuthorizationRule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/AuthorizationRules/:authorizationRuleName"
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
            "description": "Authorization rule for a namespace by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cae71c5-2538-44a2-b39d-dbf627427970"
            }
          ]
        }
      ]
    }
  ]
}