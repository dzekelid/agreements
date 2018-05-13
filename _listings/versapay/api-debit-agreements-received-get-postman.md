{
  "info": {
    "name": "VersaPay API Reference",
    "_postman_id": "a726f574-90b5-410e-88b7-abb2fc77e517",
    "description": "# IntroductionThe VersaPay API offers operations in support of its flagship products:* ARC - accounts receivable platform with automated invoicing, effective collaboration, flexible payments and cash application to improve efficiency and customer relationships.  * Importing &amp; exporting customers, invoices, and payments.  * Monitoring file based imports/batches.* PayPort - cloud based platform to electronically push and pull funds across the EFT / ACH network.  * Moving funds using transactions and pre-authorized debit agreements.  * A secure hosted checkout for accepting payments through your website or email.Please contact us at support@versapay.com for support &amp; setup of A/R invoicing integration, hosted checkout, and/or payment acceptance.## EnvironmentsThe demo environment is a useful sandbox for integration testing where transaction settlements are simulated using test account numbers and test dollar amounts.`https://demo.versapay.com`Once integration testing is complete via the demo environment, start sending your requests to the production URL to start moving money and/or integrating with VersaPay.`https://secure.versapay.com`## Rate LimitsThere is a 60 request per minute API limit. Any requests above this limit will result in HTTP return code `403 Forbidden (Rate Limit Exceeded)`.## Access to API KeysVisit your account settings in [demo](https://demo.versapay.com/account) or [production](https://secure.versapay.com/account) to setup API keys needed for authentication as well as webhooks to receive relevant callbacks from VersaPay transaction processing. You can generate/disable your API Keys as often as necessary for security reasons.If you do not have an account, please contact VersaPay Support for support &amp; setup of AR invoicing integration, hosted checkout and/or payment acceptance.# AuthenticationAPI requests are authenticated using [HTTP Basic Access Authentication](https://en.wikipedia.org/wiki/Basic_access_authentication). Simply provide the token/key values as the user and password parameters, using cURL for instance:`curl -u &quot;Nvax...:UN0I...&quot; -X POST https://secure.versapay.com/api/...`# Testing Transactions## EFT Bank Account NumbersIn the demo environment, the following test bank accounts can be setup up in your account.|Institution|Institution Number|Branch|Account Number||:--|:--|:--|:--||TD|004|99960|1-12 digits||RBC|003|16824|1-12 digits||BMO|001|99520|1-12 digits||HSBC|016|10880|1-12 digits|When VersaPay prompts you to verify these bank accounts enter a value of `1.23` for the verification amount.To determine the outcome of a transaction funded by a bank account, set the amount accordingly:|Amount|Resulting State||:--|:--||$x.10|nsfed||$x.11|completed_but_nsfed||$x.30|error||anything else|completed|## ACH Bank Account NumbersPlease contact support@versapay.com for support &amp; setup of ACH acceptance and bank account numbers that can be used for testing.## Credit Card NumbersPlease contact support@versapay.com for support &amp; setup of Credit Card acceptance and card brands/numbers that can be used for testing.# Tools## PostmanTry out the API using [Postman app](https://www.getpostman.com/), a powerful REST API client. Download the VersaPay API Reference as a Postman Collection by clicking on the button below:[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/7e34e0700a2f8c3074c6)After downloading the collection, set up and configure the environment as follows:1. Download [the sample environment file](https://developers.versapay.com/demo.postman_environment.json).2. Import the environment file in Postman.  ![Import Environment](https://developers.versapay.com/images/import_environment.png)3. Once it is imported, edit the environment to add API token and keys associated to your test account.  ![Edit Environment](https://developers.versapay.com/images/edit_environment.png)4. Click Update to save your changes.5. Before placing API calls, make sure the correct environment is selected.  ![Select Environment](https://developers.versapay.com/images/select_environment.png)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "view",
      "item": [
        {
          "id": "07b738e0-305f-4fe5-94c0-ae56e8adaa6f",
          "name": "viewReceivedAgreements",
          "request": {
            "url": "http://secure.versapay.com/api/debit_agreements/received?page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View received agreements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2848e06-f6cc-44be-9e47-65d13ecbbab6"
            }
          ]
        }
      ]
    }
  ]
}