{
  "info": {
    "name": "LogicManagementClient",
    "_postman_id": "f22e11b9-acfe-409e-bb57-6696200d776d",
    "description": "REST API for Azure Logic Apps.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "agreements",
      "item": [
        {
          "id": "15644d03-8449-43f9-97db-a14768d60d96",
          "name": "Agreements_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an integration account agreement"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34f4c2a3-5f38-40c6-a943-9d802e3de654"
            }
          ]
        }
      ]
    }
  ]
}