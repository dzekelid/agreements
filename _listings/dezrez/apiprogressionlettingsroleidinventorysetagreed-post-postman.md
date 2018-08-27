{
  "info": {
    "name": "Dezrez Sets whether inventory is agreed with tenants",
    "_postman_id": "1bd5a594-75b3-4706-a553-92abcffe4836",
    "description": "Sets whether inventory is agreed with tenants.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sets",
      "item": [
        {
          "id": "5de528bb-4e4e-41fc-9af5-6a1f06fc9998",
          "name": "LettingsProgression_SetInventoryAgreedByroleIdByagreed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/progression/lettings/:roleId/inventory/setagreed"
              ],
              "query": [
                {
                  "key": "agreed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "roleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Sets whether inventory is agreed with tenants."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6442dd46-47e7-4408-b134-2634017a9d81"
            }
          ]
        }
      ]
    }
  ]
}