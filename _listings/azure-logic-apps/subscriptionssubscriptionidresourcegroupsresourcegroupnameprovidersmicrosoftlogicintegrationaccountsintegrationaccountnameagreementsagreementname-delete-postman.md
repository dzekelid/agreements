{
  "info": {
    "name": "LogicManagementClient",
    "_postman_id": "84c052af-2977-419d-9463-63f5e983df27",
    "description": "REST API for Azure Logic Apps.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "agreements",
      "item": [
        {
          "id": "987a98d5-872f-4bbc-9a2a-95c1f9311208",
          "name": "Agreements_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Logic/integrationAccounts/:integrationAccountName/agreements/:agreementName"
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
                  "id": "agreementName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "integrationAccountName",
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
            "description": "Deletes an integration account agreement"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6162c4e-1d6a-40db-a86d-dae7d514195e"
            }
          ]
        }
      ]
    }
  ]
}