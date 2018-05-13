{
  "info": {
    "name": "Azure Virtual Network API Express Route Circuit Authorizations List",
    "_postman_id": "f32a9dd8-f2c8-4cbb-a187-3ce56080e763",
    "description": "Gets all authorizations in an express route circuit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "express route circuit authorizations",
      "item": [
        {
          "id": "12cd36c0-70d7-4a38-8fc2-55295450a772",
          "name": "ExpressRouteCircuitAuthorizations_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/expressRouteCircuits/:circuitName/authorizations"
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
            "description": "Gets all authorizations in an express route circuit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3e0fce0-c447-4c51-91fe-dad744db4fbf"
            }
          ]
        }
      ]
    }
  ]
}