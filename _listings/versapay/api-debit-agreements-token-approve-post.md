---
swagger: "2.0"
info:
  title: VersaPay Approve an Agreement
  description: Approve an agreement.
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