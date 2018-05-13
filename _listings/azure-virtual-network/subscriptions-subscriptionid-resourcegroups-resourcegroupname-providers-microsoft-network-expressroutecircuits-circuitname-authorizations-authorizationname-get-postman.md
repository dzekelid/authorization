{
  "info": {
    "name": "Azure Virtual Network API Express Route Circuit Authorizations Get",
    "_postman_id": "addaa65a-bb4a-44c6-8f85-52da579ed6a3",
    "description": "Gets the specified authorization from the specified express route circuit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "express route circuit authorizations",
      "item": [
        {
          "id": "2dffd9bc-47fd-447d-8a9a-72d083efd3c7",
          "name": "ExpressRouteCircuitAuthorizations_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/expressRouteCircuits/:circuitName/authorizations/:authorizationName"
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
                  "id": "authorizationName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "circuitName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified authorization from the specified express route circuit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbe9ee47-c24a-4a76-a629-b932e5debb99"
            }
          ]
        }
      ]
    }
  ]
}