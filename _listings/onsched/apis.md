---
name: OnSched
x-slug: onsched
description: Build secure and scalable custom apps for Online Booking. Our flexible
  API provides many options for availability and booking. OnSched is an API first
  booking software that allows you to bring your design to life by creating your own
  booking flow. Using our robust API you can customize the interaction between your
  consumers and vendors while we do all the leg work behind the scenes. Want to offer
  online booking to your vendors? Ask about our white labelling solutions and rebrand
  our software as your own.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
x-kinRank: "7"
x-alexaRank: ""
tags: Customers
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/apis.md
specificationVersion: "0.14"
apis:
- name: OnSched API - Returns a list of customers.
  x-api-slug: consumerv1customers-get
  description: "The results are returned in pages. Use the offset and limit parameters
    to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
    the other query parameters to optionally filter the results list."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customers-get-openapi.md
- name: OnSched API - Creates a new customer object.
  x-api-slug: consumerv1customers-post
  description: "Use this endpoint to create a new customer. If not specified the business
    location id defaults to the first location in the company.\r\nEmail Address and
    a lastname are required for creating a new customer."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customers-post-openapi.md
- name: OnSched API - Returns a customer object.
  x-api-slug: consumerv1customersid-get
  description: "The result returned is a single customer object. An id is required
    to find the customer. Find customer id's using either the GET consumer/v1/customers
    end point,\r\nor the GET consumer/v1/appointments end point. A customer object
    is automatically created with the first booking if it doesn't already exist."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersid-get-openapi.md
- name: OnSched API - Updates a customer object.
  x-api-slug: consumerv1customersid-put
  description: "Use this endpoint to update customer information. If not specified
    the business location id defaults to the first location in the company.\r\nBlank
    fields are not changed"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersid-put-openapi.md
- name: OnSched API - Deletes a customer subscription object.
  x-api-slug: consumerv1customersid-delete
  description: Deletes a customer subscription object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersid-delete-openapi.md
- name: OnSched API - Returns a list of customField objects
  x-api-slug: consumerv1customerscustomfields-get
  description: "This end point returns your Customer custom field definitions.\r\n\r\nCustomer
    custom fields are different than Appointment custom fields. Appointment custom
    fields are\r\nstored with each appointment. They are used when the information
    collected during the booking is specific\r\nto a particular visit, where as Customer
    custom fields are stored with the customer profile. \r\n\r\nUse the key field,
    and type to determine how to update field values\r\nin POST /consumer/v1/customers
    and PUT /consumer/v1/customers/{id}"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerscustomfields-get-openapi.md
- name: OnSched API - Returns a list of lead questions
  x-api-slug: consumerv1customersregistrationfields-get
  description: "This end point returns your Customer Registration fields.\r\n\r\nCustomer
    custom fields are different than Appointment custom fields. Appointment custom
    fields are\r\nstored with each appointment. They are used when the information
    collected during the booking is specific\r\nto a particular visit, where as Customer
    custom fields are stored with the customer profile."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersregistrationfields-get-openapi.md
- name: OnSched API - Returns a list of customers.
  x-api-slug: consumerv1customersplans-get
  description: "The results are returned in pages. Use the offset and limit parameters
    to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
    the other query parameters to optionally filter the results list."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersplans-get-openapi.md
- name: OnSched API - Returns a customer object.
  x-api-slug: consumerv1customersplansid-get
  description: "The result returned is a single customer object. An id is required
    to find the customer. Find customer id's using either the GET consumer/v1/customers
    end point,\r\nor the GET consumer/v1/appointments end point. A customer object
    is automatically created with the first booking if it doesn't already exist."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersplansid-get-openapi.md
- name: OnSched API - Returns a list of customer booking limits.
  x-api-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
  description: "The result returned is list of limit rules as defined by the subscribed
    customer plan along with Booking Counts/Minutes\r\nThe results indicate the remaining
    bookings count / minutes. Use the results in your app to determine if the customer
    should continue booking.\r\nYou can enforce Limits in periods: Daily,Weekly,Monthly
    and for maximum total limits. Maximum total limits is based on six months prior
    to\r\nthe DateTimeTz and six months after the DateTimeTz. Daily, Weekly and Monthly
    limits are based on the calculated period relative to the\r\nsubscription plan
    start. Daily,Weekly and Monthly limits can be setup on a per interval basis e.g.
    to biweekly, or daily every 10 days.\r\nSee customer plans setup in the Portal
    for more information.\r\nAll parameters are required. If resourceId is not applicable
    for a non-resource calendar, pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get-openapi.md
- name: OnSched API - Returns a list of customer subscriptions.
  x-api-slug: consumerv1customerssubscriptions-get
  description: "The results are returned in pages. Use the offset and limit parameters
    to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
    the other query parameters to optionally filter the results list."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerssubscriptions-get-openapi.md
- name: OnSched API - Returns a customer subscription object.
  x-api-slug: consumerv1customersidsubscriptions-get
  description: The result returned is a single customer subscription object. A customer
    can only be subsribed to a single Customer Plan
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersidsubscriptions-get-openapi.md
- name: OnSched API - Creates a new customer subscription object.
  x-api-slug: consumerv1customersidsubscriptions-post
  description: Use this endpoint to create a new customer subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersidsubscriptions-post-openapi.md
- name: OnSched API - Returns a customer subscription object.
  x-api-slug: consumerv1customerssubscriptionsid-get
  description: The result returned is a single customer subscription object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerssubscriptionsid-get-openapi.md
- name: OnSched API - Updates a customer subscription object.
  x-api-slug: consumerv1customerssubscriptionsid-put
  description: Use this endpoint to update customer subscription information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerssubscriptionsid-put-openapi.md
- name: OnSched API - Deletes a list of lead questions
  x-api-slug: consumerv1customerssubscriptionsid-delete
  description: Deletes a list of lead questions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerssubscriptionsid-delete-openapi.md
- name: OnSched API - Returns a list of country objects
  x-api-slug: consumerv1customerscountries-get
  description: Returns a list of countries with the associated country code. Country
    codes are based on the 2 character ANSI standard.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerscountries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customerscountries-get-openapi.md
- name: OnSched API - Returns a list of state objects
  x-api-slug: consumerv1customersstates-get
  description: "Returns a list of states with the associated state code and country.
    \r\n\r\nContact us if states for your countries of operation are not currently
    loaded."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/onsched-logo.png
  humanURL: http://www.onsched.com
  baseURL: https://api.onsched.com//
  tags: API Provider, Bookings, Profiles, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/onsched/consumerv1customersstates-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://onenote.api.gallery.streamdata.io
- type: x-api-stack
  url: http://onsched.stack.network
- type: x-documentation
  url: https://www.onsched.com/api/docs/
- type: x-pricing
  url: https://www.onsched.com/index.html#self-service
- type: x-website
  url: http://www.onsched.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---