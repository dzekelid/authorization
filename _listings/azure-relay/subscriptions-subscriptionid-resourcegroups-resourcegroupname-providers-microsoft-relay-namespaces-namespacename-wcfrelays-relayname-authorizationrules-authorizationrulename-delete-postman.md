{
  "info": {
    "name": "Azure Relay API WCFRelays Delete Authorization Rule",
    "_postman_id": "2a6dccc2-9247-4719-beca-df08f585d2a1",
    "description": "Deletes a WCFRelays authorization rule",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "wcfrelays authorization rule",
      "item": [
        {
          "id": "e3abb4e9-b5f0-4df3-bbb1-e6efb83e5299",
          "name": "WCFRelays_DeleteAuthorizationRule",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a WCFRelays authorization rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3ce47f7-1101-4223-a13b-7421110489f5"
            }
          ]
        }
      ]
    }
  ]
}