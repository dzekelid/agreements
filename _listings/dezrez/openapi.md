---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/lettings/{roleId}/inventory/setagreed:
    post:
      summary: Sets whether inventory is agreed with tenants
      description: Sets whether inventory is agreed with tenants.
      operationId: LettingsProgression_SetInventoryAgreedByroleIdByagreed
      x-api-path-slug: apiprogressionlettingsroleidinventorysetagreed-post
      parameters:
      - in: query
        name: agreed
        description: Is inventory agreed
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Tenant role id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Whether
      - Inventory
      - Is
      - Agreed
      - Tenants
  /api/documentgeneration/tenancyagreementast:
    post:
      summary: Generates Tenancy Agreement correspondence
      description: Generates tenancy agreement correspondence.
      operationId: DocumentGeneration_TenancyAgreementASTBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationtenancyagreementast-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Tenancy
      - Agreement
      - Correspondence
  /api/tenancy/{id}/setagreement:
    post:
      summary: Set Agreement type for the tenancy.
      description: Set agreement type for the tenancy..
      operationId: Tenancy_SetAgreementByidByagreementDataContract
      x-api-path-slug: apitenancyidsetagreement-post
      parameters:
      - in: body
        name: agreementDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Tenant Role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Agreement
      - Typethe
      - Tenancy
---