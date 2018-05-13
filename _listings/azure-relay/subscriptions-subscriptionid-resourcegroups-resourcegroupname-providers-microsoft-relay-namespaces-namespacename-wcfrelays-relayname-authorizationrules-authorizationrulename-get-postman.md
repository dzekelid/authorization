{
  "info": {
    "name": "Azure Relay API WCFRelays Get Authorization Rule",
    "_postman_id": "aafc2407-5e94-45c0-92dc-a4486c2e43a7",
    "description": "Get authorizationRule for a WCFRelays by name.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "wcfrelays authorization rule",
      "item": [
        {
          "id": "de263de6-f708-447d-a8f8-5f6fdcacd749",
          "name": "WCFRelays_GetAuthorizationRule",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/WcfRelays/:relayName/authorizationRules/:authorizationRuleName"
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
                  "id": "relayName",
                  "value": "relayName",
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
            "description": "Get authorizationRule for a WCFRelays by name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ff2a8b8-bb49-49da-ad05-3cca8ea53756"
            }
          ]
        }
      ]
    }
  ]
}