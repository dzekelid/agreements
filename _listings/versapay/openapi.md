---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 1
info:
  title: VersaPay API Reference
  description: -introductionthe-versapay-api-offers-operations-in-support-of-its-flagship-products-arc--accounts-receivable-platform-with-automated-invoicing-effective-collaboration-flexible-payments-and-cash-application-to-improve-efficiency-and-customer-relationships---importing--exporting-customers-invoices-and-payments---monitoring-file-based-importsbatches-payport--cloud-based-platform-to-electronically-push-and-pull-funds-across-the-eft--ach-network---moving-funds-using-transactions-and-preauthorized-debit-agreements---a-secure-hosted-checkout-for-accepting-payments-through-your-website-or-emailplease-contact-us-at-supportversapaycom-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance-environmentsthe-demo-environment-is-a-useful-sandbox-for-integration-testing-where-transaction-settlements-are-simulated-using-test-account-numbers-and-test-dollar-amountshttpsdemoversapaycomonce-integration-testing-is-complete-via-the-demo-environment-start-sending-your-requests-to-the-production-url-to-start-moving-money-andor-integrating-with-versapayhttpssecureversapaycom-rate-limitsthere-is-a-60-request-per-minute-api-limit-any-requests-above-this-limit-will-result-in-http-return-code-403-forbidden-rate-limit-exceeded-access-to-api-keysvisit-your-account-settings-in-demohttpsdemoversapaycomaccount-or-productionhttpssecureversapaycomaccount-to-setup-api-keys-needed-for-authentication-as-well-as-webhooks-to-receive-relevant-callbacks-from-versapay-transaction-processing-you-can-generatedisable-your-api-keys-as-often-as-necessary-for-security-reasonsif-you-do-not-have-an-account-please-contact-versapay-support-for-support--setup-of-ar-invoicing-integration-hosted-checkout-andor-payment-acceptance-authenticationapi-requests-are-authenticated-using-http-basic-access-authenticationhttpsenwikipediaorgwikibasic-access-authentication-simply-provide-the-tokenkey-values-as-the-user-and-password-parameters-using-curl-for-instancecurl-u-nvaxun0i-x-post-httpssecureversapaycomapi-testing-transactions-eft-bank-account-numbersin-the-demo-environment-the-following-test-bank-accounts-can-be-setup-up-in-your-accountinstitutioninstitution-numberbranchaccount-numbertd00499960112-digitsrbc00316824112-digitsbmo00199520112-digitshsbc01610880112-digitswhen-versapay-prompts-you-to-verify-these-bank-accounts-enter-a-value-of-123-for-the-verification-amountto-determine-the-outcome-of-a-transaction-funded-by-a-bank-account-set-the-amount-accordinglyamountresulting-statex10nsfedx11completed-but-nsfedx30erroranything-elsecompleted-ach-bank-account-numbersplease-contact-supportversapaycom-for-support--setup-of-ach-acceptance-and-bank-account-numbers-that-can-be-used-for-testing-credit-card-numbersplease-contact-supportversapaycom-for-support--setup-of-credit-card-acceptance-and-card-brandsnumbers-that-can-be-used-for-testing-tools-postmantry-out-the-api-using-postman-apphttpswwwgetpostmancom-a-powerful-rest-api-client-download-the-versapay-api-reference-as-a-postman-collection-by-clicking-on-the-button-belowrun-in-postmanhttpsrunpstmniobuttonsvghttpsappgetpostmancomruncollection7e34e0700a2f8c3074c6after-downloading-the-collection-set-up-and-configure-the-environment-as-follows1-download-the-sample-environment-filehttpsdevelopersversapaycomdemopostman-environmentjson2-import-the-environment-file-in-postman--import-environmenthttpsdevelopersversapaycomimagesimport-environmentpng3-once-it-is-imported-edit-the-environment-to-add-api-token-and-keys-associated-to-your-test-account--edit-environmenthttpsdevelopersversapaycomimagesedit-environmentpng4-click-update-to-save-your-changes5-before-placing-api-calls-make-sure-the-correct-environment-is-selected--select-environmenthttpsdevelopersversapaycomimagesselect-environmentpng
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
  /api/debit_agreements:
    post:
      summary: Create an Agreement
      description: Create an agreement.
      operationId: createAgreement
      x-api-path-slug: apidebit-agreements-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Create
      - ""
      - Agreementss
  /api/debit_agreements/sent:
    get:
      summary: View Sent Agreements
      description: View sent agreements.
      operationId: viewSentAgreements
      x-api-path-slug: apidebit-agreementssent-get
      parameters:
      - in: query
        name: page
        description: 50 items are displayed per page
      responses:
        200:
          description: OK
      tags:
      - View
      - Sent
      - Agreements
  /api/debit_agreements/received:
    get:
      summary: View Received Agreements
      description: View received agreements.
      operationId: viewReceivedAgreements
      x-api-path-slug: apidebit-agreementsreceived-get
      parameters:
      - in: query
        name: page
        description: 50 items are displayed per page
      responses:
        200:
          description: OK
      tags:
      - View
      - Received
      - Agreements
  /api/debit_agreements/{token}/approve:
    post:
      summary: Approve an Agreement
      description: Approve an agreement.
      operationId: approveAgreement
      x-api-path-slug: apidebit-agreementstokenapprove-post
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
      - Approve
      - Agreements
  /api/debit_agreements/{token}/cancel:
    post:
      summary: Cancel an Agreement
      description: Cancel an agreement.
      operationId: cancelAgreement
      x-api-path-slug: apidebit-agreementstokencancel-post
      parameters:
      - in: path
        name: token
        description: The agreement identifier
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Agreements
  /api/debit_agreements/{token}/reject:
    post:
      summary: Reject an Agreement
      description: Reject a *pending* agreement by supplying an agreement's *token*
        attribute and providing a *rejection_reason*.
      operationId: rejectAgreement
      x-api-path-slug: apidebit-agreementstokenreject-post
      parameters:
      - in: path
        name: token
        description: The agreement identifier
      responses:
        200:
          description: OK
      tags:
      - Reject
      - Agreements
  /api/debit_agreements/{token}/revoke:
    post:
      summary: Revoke an Agreement
      description: Revoke an *approved* agreement for your account by supplying an
        agreement's token attribute. The agreement's creator will no longer be able
        to debit your account using this agreement.
      operationId: revokeAgreement
      x-api-path-slug: apidebit-agreementstokenrevoke-post
      parameters:
      - in: path
        name: token
        description: The agreement identifier
      responses:
        200:
          description: OK
      tags:
      - Revoke
      - Agreements
  /authorize:
    get:
      summary: Debit Agreement Hosted Checkout
      description: |-
        Clients, customers, or donors, for instance, can initiate a pre-authorized debit agreement by clicking a link on your website or in an email.
        <br>
        `https://secure.versapay.com/authorize?api_token={your_api_token}&message={explanation_of_what_this_is_for}`
        <br>
      operationId: clients-customers-or-donors-for-instance-can-initiate-a-preauthorized-debit-agreement-by-clicking-a-
      x-api-path-slug: authorize-get
      parameters:
      - in: query
        name: api_token
        description: A valid API token generated from your account
      - in: query
        name: message
        description: A message for the user describing the pre-authorized debit agreement
      - in: query
        name: reference
        description: Extra data (max 255 characters)
      - in: query
        name: return_to
        description: A url which will displayed to the user to return to your website
          after they finish the Signup and Confirmation
      responses:
        200:
          description: OK
      tags:
      - Debit
      - ""
      - Agreements
      - Hosted
      - Checkout
---