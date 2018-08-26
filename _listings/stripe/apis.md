---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripes payment platform to accept
  and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1914"
tags: Customers
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe - Get Customers
  x-api-slug: customers-get
  description: Returns a list of your customers. The customers are returned sorted
    by creation date, with the most recent customers appearing first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customers-get-openapi.md
- name: Stripe - Get Customers Customer
  x-api-slug: customerscustomer-get
  description: Retrieves the details of an existing customer. You need only supply
    the unique customer identifier that was returned upon customer creation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accounts-get
  description: You can see a list of the bank accounts belonging to a Customer. Note
    that the 10 most recent sources are always available by default on the Customer.
    If you need more than those 10, you can use this API method and the limit and
    starting_after parameters to page through additional bank accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accountsid-get
  description: By default, you can see the 10 most recent sources stored on a Customer
    directly on the object, but you can also retrieve details about a specific bank
    account stored on the Stripe account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercards-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercardsid-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-openapi.md
- name: Stripe - Get Customers Customer Discount
  x-api-slug: customerscustomerdiscount-get
  description: Get Customers, Customer, Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersources-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersourcesid-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions
  x-api-slug: customerscustomersubscriptions-get
  description: You can see a list of the customer???s active subscriptions. Note that
    the 10 most recent active subscriptions are always available by default on the
    customer object. If you need more than those 10, you can use the limit and starting_after
    parameters to page through additional subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Get Customers Customer
  x-api-slug: customerscustomer-get
  description: Retrieves the details of an existing customer. You need only supply
    the unique customer identifier that was returned upon customer creation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accounts-get
  description: You can see a list of the bank accounts belonging to a Customer. Note
    that the 10 most recent sources are always available by default on the Customer.
    If you need more than those 10, you can use this API method and the limit and
    starting_after parameters to page through additional bank accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accountsid-get
  description: By default, you can see the 10 most recent sources stored on a Customer
    directly on the object, but you can also retrieve details about a specific bank
    account stored on the Stripe account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercards-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercardsid-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-openapi.md
- name: Stripe - Get Customers Customer Discount
  x-api-slug: customerscustomerdiscount-get
  description: Get Customers, Customer, Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersources-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersourcesid-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions
  x-api-slug: customerscustomersubscriptions-get
  description: You can see a list of the customer???s active subscriptions. Note that
    the 10 most recent active subscriptions are always available by default on the
    customer object. If you need more than those 10, you can use the limit and starting_after
    parameters to page through additional subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
- name: Stripe - Get Customers Customer
  x-api-slug: customerscustomer-get
  description: Retrieves the details of an existing customer. You need only supply
    the unique customer identifier that was returned upon customer creation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomer-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accounts-get
  description: You can see a list of the bank accounts belonging to a Customer. Note
    that the 10 most recent sources are always available by default on the Customer.
    If you need more than those 10, you can use this API method and the limit and
    starting_after parameters to page through additional bank accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accounts-get-openapi.md
- name: Stripe - Get Customers Customer Bank Accounts
  x-api-slug: customerscustomerbank-accountsid-get
  description: By default, you can see the 10 most recent sources stored on a Customer
    directly on the object, but you can also retrieve details about a specific bank
    account stored on the Stripe account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerbank-accountsid-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercards-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercards-get-openapi.md
- name: Stripe - Get Customers Customer Cards
  x-api-slug: customerscustomercardsid-get
  description: Get Customers, Customer, Cards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomercardsid-get-openapi.md
- name: Stripe - Get Customers Customer Discount
  x-api-slug: customerscustomerdiscount-get
  description: Get Customers, Customer, Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomerdiscount-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersources-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersources-get-openapi.md
- name: Stripe - Get Customers Customer Sources
  x-api-slug: customerscustomersourcesid-get
  description: Get Customers, Customer, Sources
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersourcesid-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions
  x-api-slug: customerscustomersubscriptions-get
  description: You can see a list of the customer???s active subscriptions. Note that
    the 10 most recent active subscriptions are always available by default on the
    customer object. If you need more than those 10, you can use the limit and starting_after
    parameters to page through additional subscriptions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptions-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed
  x-api-slug: customerscustomersubscriptionssubscription-exposed-id-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-id-get-openapi.md
- name: Stripe - Get Customers Customer Subscriptions Subscription Exposed  Discount
  x-api-slug: customerscustomersubscriptionssubscription-exposed-iddiscount-get
  description: Get Customers, Customer, Subscriptions, Subscription, Exposed, , Discount
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Billing, Finance, Payments, Payments, Stripe Stack, Imports, Change Log Example,
    Stack Network, Stack, SaaS, Invoices, Payments, Relative Data, Service API, Relative
    StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/stripe/customerscustomersubscriptionssubscription-exposed-iddiscount-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://stride.api.gallery.streamdata.io
- type: x-api-stack
  url: http://stripe.stack.network
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-email
  url: dpo@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-linkedin
  url: https://www.linkedin.com/company/stripe/
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---