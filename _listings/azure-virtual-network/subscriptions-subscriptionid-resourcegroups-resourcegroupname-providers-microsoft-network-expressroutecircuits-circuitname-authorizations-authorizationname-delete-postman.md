{
  "info": {
    "name": "Azure Virtual Network API Express Route Circuit Authorizations Delete",
    "_postman_id": "752b4c40-d663-472a-83c5-a8240f1676d3",
    "description": "Deletes the specified authorization from the specified express route circuit.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "express route circuit authorizations",
      "item": [
        {
          "id": "ea9b9caf-682d-4b60-97bb-b13a5fefe17b",
          "name": "ExpressRouteCircuitAuthorizations_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified authorization from the specified express route circuit"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3191c8ed-ed4f-4a1f-bd8d-cec68df74009"
            }
          ]
        }
      ]
    }
  ]
}