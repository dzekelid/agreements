---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Get User Agreement
  description: The GetUserAgreement API operation lets you retrieve the user agreement
    for the customer to approve the new PayPal account.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptiveAccounts/GetUserAgreement:
    post:
      summary: Get User Agreement
      description: The GetUserAgreement API operation lets you retrieve the user agreement
        for the customer to approve the new PayPal account.
      operationId: AdaptiveAccounts.GetUserAgreement.post
      x-api-path-slug: adaptiveaccountsgetuseragreement-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Aggreements
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