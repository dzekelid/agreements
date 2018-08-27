---
name: VersaPay
x-slug: versapay
description: VersaPay handles elements of both credit and debit card merchant payment
  processing in Canada. In offering a host of merchant account services and credit
  card POS terminals it allows for an efficient merchant payment service in all aspects-
  in person, on the go, online, and at the office. Founded in 2005 by Michael Gokturk,
  VersaPay is a Canadian owned and operated national financial transaction services
  provider partnered with Chase Paymentech. Versapay also offers electronic funds
  transfer through a system called Versapay EMT.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
x-kinRank: "9"
x-alexaRank: "410909"
tags: Agreements
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apis.md
specificationVersion: "0.14"
apis:
- name: VersaPay API Reference - View Sent Agreements
  x-api-slug: apidebit-agreementssent-get
  description: View sent agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-openapi.md
- name: VersaPay API Reference - View Received Agreements
  x-api-slug: apidebit-agreementsreceived-get
  description: View received agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-openapi.md
- name: VersaPay API Reference - Approve an Agreement
  x-api-slug: apidebit-agreementstokenapprove-post
  description: Approve an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenapprove-post-openapi.md
- name: VersaPay API Reference - Cancel an Agreement
  x-api-slug: apidebit-agreementstokencancel-post
  description: Cancel an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-openapi.md
- name: VersaPay API Reference - Reject an Agreement
  x-api-slug: apidebit-agreementstokenreject-post
  description: Reject a *pending* agreement by supplying an agreement's *token* attribute
    and providing a *rejection_reason*.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-openapi.md
- name: VersaPay API Reference - Revoke an Agreement
  x-api-slug: apidebit-agreementstokenrevoke-post
  description: Revoke an *approved* agreement for your account by supplying an agreement's
    token attribute. The agreement's creator will no longer be able to debit your
    account using this agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-openapi.md
- name: VersaPay API Reference - Debit Agreement Hosted Checkout
  x-api-slug: authorize-get
  description: |-
    Clients, customers, or donors, for instance, can initiate a pre-authorized debit agreement by clicking a link on your website or in an email.
    <br>
    `https://secure.versapay.com/authorize?api_token={your_api_token}&message={explanation_of_what_this_is_for}`
    <br>
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/authorize-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/authorize-get-openapi.md
- name: VersaPay API Reference - Create an Agreement
  x-api-slug: apidebit-agreements-post
  description: Create an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreements-post-openapi.md
- name: VersaPay API Reference - View Received Agreements
  x-api-slug: apidebit-agreementsreceived-get
  description: View received agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-openapi.md
- name: VersaPay API Reference - View Sent Agreements
  x-api-slug: apidebit-agreementssent-get
  description: View sent agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-openapi.md
- name: VersaPay API Reference - Approve an Agreement
  x-api-slug: apidebit-agreementstokenapprove-post
  description: Approve an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenapprove-post-openapi.md
- name: VersaPay API Reference - Cancel an Agreement
  x-api-slug: apidebit-agreementstokencancel-post
  description: Cancel an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-openapi.md
- name: VersaPay API Reference - Reject an Agreement
  x-api-slug: apidebit-agreementstokenreject-post
  description: Reject a *pending* agreement by supplying an agreement's *token* attribute
    and providing a *rejection_reason*.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-openapi.md
- name: VersaPay API Reference - Revoke an Agreement
  x-api-slug: apidebit-agreementstokenrevoke-post
  description: Revoke an *approved* agreement for your account by supplying an agreement's
    token attribute. The agreement's creator will no longer be able to debit your
    account using this agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-openapi.md
- name: VersaPay API Reference - Create an Agreement
  x-api-slug: apidebit-agreements-post
  description: Create an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreements-post-openapi.md
- name: VersaPay API Reference - View Received Agreements
  x-api-slug: apidebit-agreementsreceived-get
  description: View received agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementsreceived-get-openapi.md
- name: VersaPay API Reference - View Sent Agreements
  x-api-slug: apidebit-agreementssent-get
  description: View sent agreements.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementssent-get-openapi.md
- name: VersaPay API Reference - Approve an Agreement
  x-api-slug: apidebit-agreementstokenapprove-post
  description: Approve an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenapprove-post-openapi.md
- name: VersaPay API Reference - Cancel an Agreement
  x-api-slug: apidebit-agreementstokencancel-post
  description: Cancel an agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokencancel-post-openapi.md
- name: VersaPay API Reference - Reject an Agreement
  x-api-slug: apidebit-agreementstokenreject-post
  description: Reject a *pending* agreement by supplying an agreement's *token* attribute
    and providing a *rejection_reason*.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenreject-post-openapi.md
- name: VersaPay API Reference - Revoke an Agreement
  x-api-slug: apidebit-agreementstokenrevoke-post
  description: Revoke an *approved* agreement for your account by supplying an agreement's
    token attribute. The agreement's creator will no longer be able to debit your
    account using this agreement.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1208-versapay-corporation.jpg
  humanURL: http://developers.versapay.com/index.html
  baseURL: https://secure.versapay.com//
  tags: Billing, Checking, Payments, Payments, Stack Network, Financial Services,
    Technology, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/agreements/master/_listings/versapay/apidebit-agreementstokenrevoke-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://venmo.api.gallery.streamdata.io
- type: x-api-stack
  url: http://versapay.stack.network
- type: x-base
  url: https://secure.versapay.com/api/
- type: x-blog
  url: https://www.versapay.com/blog/
- type: x-blog-rss
  url: http://www.versapay.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/versapay
- type: x-crunchbase
  url: https://crunchbase.com/organization/versapay
- type: x-github
  url: https://github.com/versapay
- type: x-partners
  url: https://www.versapay.com/partners/
- type: x-support
  url: https://www.versapay.com/support/
- type: x-twitter
  url: https://twitter.com/VersaPay
- type: x-website
  url: http://developers.versapay.com/index.html
- type: x-website
  url: https://www.versapay.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---