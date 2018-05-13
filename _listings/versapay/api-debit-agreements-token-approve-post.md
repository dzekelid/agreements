---
swagger: "2.0"
info:
  title: VersaPay API Reference
  description: '# IntroductionThe VersaPay API offers operations in support of its
    flagship products:* ARC - accounts receivable platform with automated invoicing,
    effective collaboration, flexible payments and cash application to improve efficiency
    and customer relationships.  * Importing &amp; exporting customers, invoices,
    and payments.  * Monitoring file based imports/batches.* PayPort - cloud based
    platform to electronically push and pull funds across the EFT / ACH network.  *
    Moving funds using transactions and pre-authorized debit agreements.  * A secure
    hosted checkout for accepting payments through your website or email.Please contact
    us at support@versapay.com for support &amp; setup of A/R invoicing integration,
    hosted checkout, and/or payment acceptance.## EnvironmentsThe demo environment
    is a useful sandbox for integration testing where transaction settlements are
    simulated using test account numbers and test dollar amounts.`https://demo.versapay.com`Once
    integration testing is complete via the demo environment, start sending your requests
    to the production URL to start moving money and/or integrating with VersaPay.`https://secure.versapay.com`##
    Rate LimitsThere is a 60 request per minute API limit. Any requests above this
    limit will result in HTTP return code `403 Forbidden (Rate Limit Exceeded)`.##
    Access to API KeysVisit your account settings in [demo](https://demo.versapay.com/account)
    or [production](https://secure.versapay.com/account) to setup API keys needed
    for authentication as well as webhooks to receive relevant callbacks from VersaPay
    transaction processing. You can generate/disable your API Keys as often as necessary
    for security reasons.If you do not have an account, please contact VersaPay Support
    for support &amp; setup of AR invoicing integration, hosted checkout and/or payment
    acceptance.# AuthenticationAPI requests are authenticated using [HTTP Basic Access
    Authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). Simply
    provide the token/key values as the user and password parameters, using cURL for
    instance:`curl -u &quot;Nvax...:UN0I...&quot; -X POST https://secure.versapay.com/api/...`#
    Testing Transactions## EFT Bank Account NumbersIn the demo environment, the following
    test bank accounts can be setup up in your account.|Institution|Institution Number|Branch|Account
    Number||:--|:--|:--|:--||TD|004|99960|1-12 digits||RBC|003|16824|1-12 digits||BMO|001|99520|1-12
    digits||HSBC|016|10880|1-12 digits|When VersaPay prompts you to verify these bank
    accounts enter a value of `1.23` for the verification amount.To determine the
    outcome of a transaction funded by a bank account, set the amount accordingly:|Amount|Resulting
    State||:--|:--||$x.10|nsfed||$x.11|completed_but_nsfed||$x.30|error||anything
    else|completed|## ACH Bank Account NumbersPlease contact support@versapay.com
    for support &amp; setup of ACH acceptance and bank account numbers that can be
    used for testing.## Credit Card NumbersPlease contact support@versapay.com for
    support &amp; setup of Credit Card acceptance and card brands/numbers that can
    be used for testing.# Tools## PostmanTry out the API using [Postman app](https://www.getpostman.com/),
    a powerful REST API client. Download the VersaPay API Reference as a Postman Collection
    by clicking on the button below:[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/7e34e0700a2f8c3074c6)After
    downloading the collection, set up and configure the environment as follows:1.
    Download [the sample environment file](https://developers.versapay.com/demo.postman_environment.json).2.
    Import the environment file in Postman.  ![Import Environment](https://developers.versapay.com/images/import_environment.png)3.
    Once it is imported, edit the environment to add API token and keys associated
    to your test account.  ![Edit Environment](https://developers.versapay.com/images/edit_environment.png)4.
    Click Update to save your changes.5. Before placing API calls, make sure the correct
    environment is selected.  ![Select Environment](https://developers.versapay.com/images/select_environment.png)'
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/debit_agreements/{token}/approve:
    post:
      summary: Approve an Agreement
      description: Approve an agreement
      operationId: approveAgreement
      parameters:
      - in: body
        name: fund_token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: token
        description: The agreement identifier
      responses:
        200:
          description: OK
      tags:
      - approve
      - agreements
definitions:
  FundSource:
    properties:
      type:
        description: This is a default description.
        type: get
      token:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
  Transaction:
    properties:
      transaction_type:
        description: This is a default description.
        type: get
      amount_in_cents:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      transaction_reference:
        description: This is a default description.
        type: get
      unique_reference:
        description: This is a default description.
        type: get
      process_on:
        description: This is a default description.
        type: get
      auto_withdraw:
        description: This is a default description.
        type: get
  TransactionResponse:
    properties:
      token:
        description: This is a default description.
        type: get
      amount_in_cents:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      from_account:
        description: This is a default description.
        type: get
      to_account:
        description: This is a default description.
        type: get
      from_fund:
        description: This is a default description.
        type: get
      to_fund:
        description: This is a default description.
        type: get
      transaction_reference:
        description: This is a default description.
        type: get
  Agreement:
    properties:
      token:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      created_by_user:
        description: This is a default description.
        type: get
      created_by_account:
        description: This is a default description.
        type: get
      reference:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      rejection_reason:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  Customer:
    properties:
      identifier:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      first_name:
        description: This is a default description.
        type: get
      last_name:
        description: This is a default description.
        type: get
      notes:
        description: This is a default description.
        type: get
      address_1:
        description: This is a default description.
        type: get
      address_2:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      province:
        description: This is a default description.
        type: get
  Contact:
    properties:
      email:
        description: This is a default description.
        type: get
      first_name:
        description: This is a default description.
        type: get
      last_name:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      department:
        description: This is a default description.
        type: get
      telephone:
        description: This is a default description.
        type: get
  Invoice:
    properties:
      number:
        description: This is a default description.
        type: get
      display_number:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      subtotal_tax1:
        description: This is a default description.
        type: get
      subtotal_tax2:
        description: This is a default description.
        type: get
      customer_identifier:
        description: This is a default description.
        type: get
      date:
        description: This is a default description.
        type: get
      order_date:
        description: This is a default description.
        type: get
      due_date:
        description: This is a default description.
        type: get
  LineItem:
    properties:
      number:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      quantity:
        description: This is a default description.
        type: get
      unit_cost_cents:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      balance_cents:
        description: This is a default description.
        type: get
  PaymentImport:
    properties:
      identifier:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      date:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      invoice_number:
        description: This is a default description.
        type: get
      payment_code:
        description: This is a default description.
        type: get
      payment_description:
        description: This is a default description.
        type: get
      payment_amount_attributes:
        description: This is a default description.
        type: get
      division:
        description: This is a default description.
        type: get
      customer_identifier:
        description: This is a default description.
        type: get
  FileImport:
    properties:
      id:
        description: This is a default description.
        type: get
      file_name:
        description: This is a default description.
        type: get
      file_size:
        description: This is a default description.
        type: get
      file_content_type:
        description: This is a default description.
        type: get
      file_fingerprint:
        description: This is a default description.
        type: get
      error:
        description: This is a default description.
        type: get
      result_message:
        description: This is a default description.
        type: get
      complete_at:
        description: This is a default description.
        type: get
  PaymentExport:
    properties:
      payment_reference:
        description: This is a default description.
        type: get
      invoice_number:
        description: This is a default description.
        type: get
      date:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      plan_fee:
        description: This is a default description.
        type: get
      payment_amount:
        description: This is a default description.
        type: get
      payment_transaction_amount:
        description: This is a default description.
        type: get
      payment_method:
        description: This is a default description.
        type: get
      payment_from_bank_account:
        description: This is a default description.
        type: get
      payment_from_credit_card:
        description: This is a default description.
        type: get
  Dispute:
    properties:
      closed_at:
        description: This is a default description.
        type: get
      opened_at:
        description: This is a default description.
        type: get
      opener:
        description: This is a default description.
        type: get
      closer:
        description: This is a default description.
        type: get
      opening_comment_text:
        description: This is a default description.
        type: get
      closing_comment_text:
        description: This is a default description.
        type: get
      invoice_number:
        description: This is a default description.
        type: get
      invoice_amount_paid:
        description: This is a default description.
        type: get
      invoice_balance:
        description: This is a default description.
        type: get
      dispute_reason_identifier:
        description: This is a default description.
        type: get
  inline_response_401:
    properties:
      error:
        description: This is a default description.
        type: get
  fund_token:
    properties:
      fund_token:
        description: This is a default description.
        type: get
  inline_response_412:
    properties:
      error:
        description: This is a default description.
        type: get
  body:
    properties:
      email:
        description: This is a default description.
        type: get
      reference:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  fund_token_1:
    properties:
      fund_token:
        description: This is a default description.
        type: get
  inline_response_201:
    properties:
      identifier:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  inline_response_201_1:
    properties:
      identifier:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  inline_response_201_2:
    properties:
      identifier:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  inline_response_200:
    properties:
      payment_amounts:
        description: This is a default description.
        type: get
  Invoice_adjustments_attributes:
    properties:
      label:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
  PaymentImport_payment_amount_attributes:
    properties:
      invoice_number:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      notes:
        description: This is a default description.
        type: get
      purchase_order_number:
        description: This is a default description.
        type: get
      ref1:
        description: This is a default description.
        type: get
      ref2:
        description: This is a default description.
        type: get
      ref3:
        description: This is a default description.
        type: get
x-collection-name: VersaPay
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