---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 0
info:
  title: Azure Logic Apps API Agreements Create Or Update
  description: Creates or updates an integration account agreement.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/agreements
  : get:
      summary: Agreements List By Integration Accounts
      description: Gets a list of integration account agreements.
      operationId: Agreements_ListByIntegrationAccounts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreements-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of items to be included in the result
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Agreements Integration Accounts
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/agreements/{agreementName}
  : get:
      summary: Agreements Get
      description: Gets an integration account agreement.
      operationId: Agreements_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreementsagreementname-get
      parameters:
      - in: path
        name: agreementName
        description: The integration account agreement name
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Agreements
    put:
      summary: Agreements Create Or Update
      description: Creates or updates an integration account agreement.
      operationId: Agreements_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnameagreementsagreementname-put
      parameters:
      - in: body
        name: agreement
        description: The integration account agreement
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: agreementName
        description: The integration account agreement name
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Agreements
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---