{
  "info": {
    "name": "Azure Service Bus API Topics List Authorization Rules",
    "_postman_id": "6babe23f-61b8-44fa-adfe-014d94a46b0f",
    "description": "Gets authorization rules for a topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "topics authorization rules",
      "item": [
        {
          "id": "de3a476a-9a7b-42ce-baff-826dd9a9fd59",
          "name": "Topics_ListAuthorizationRules",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ServiceBus/namespaces/:namespaceName/topics/:topicName/authorizationRules"
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
                  "id": "topicName",
                  "value": "topicName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets authorization rules for a topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8774642-2c63-4d00-be1c-924ee229ab88"
            }
          ]
        }
      ]
    }
  ]
}