{
  "info": {
    "name": "Azure Event Hubs API Event Hubs List Authorization Rules",
    "_postman_id": "5eb887f6-7cdf-491f-bc7c-d0ef92af1170",
    "description": "Gets the authorization rules for an Event Hub.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "event hubs authorization rules",
      "item": [
        {
          "id": "5cbc38d9-24dd-4d14-9490-e99b7e852367",
          "name": "EventHubs_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.EventHub/namespaces/:namespaceName/eventhubs/:eventHubName/authorizationRules"
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
                  "id": "eventHubName",
                  "value": "eventHubName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the authorization rules for an Event Hub"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8d4461d-accf-472d-887f-879ac8499728"
            }
          ]
        }
      ]
    }
  ]
}