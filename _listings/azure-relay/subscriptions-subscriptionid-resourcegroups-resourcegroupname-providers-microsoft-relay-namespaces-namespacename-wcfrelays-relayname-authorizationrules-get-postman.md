{
  "info": {
    "name": "Azure Relay API WCFRelays List Authorization Rules",
    "_postman_id": "8eb0d532-de56-4051-af46-27aa405a113a",
    "description": "Authorization rules for a WCFRelays.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "wcfrelays authorization rules",
      "item": [
        {
          "id": "d4906258-1788-423a-8dc8-dc8ba9794642",
          "name": "WCFRelays_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Relay/namespaces/:namespaceName/WcfRelays/:relayName/authorizationRules"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authorization rules for a WCFRelays"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c972a5a-237b-413a-a5ee-2124a5547a2f"
            }
          ]
        }
      ]
    }
  ]
}