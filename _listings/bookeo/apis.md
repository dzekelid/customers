---
name: Bookeo
x-slug: bookeo
description: Bookeo provides a leading online booking and scheduling system for tours,
  classes, and appointments, to help you save money and time. Click to learn more!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
x-kinRank: "7"
x-alexaRank: "23042"
tags: Customers
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/apis.md
specificationVersion: "0.14"
apis:
- name: Bookeo - Retrieve customers
  x-api-slug: customers-get
  description: Get a list of customers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customers-get-openapi.md
- name: Bookeo - Create a new customer.
  x-api-slug: customers-post
  description: |-
    Create a new customer.
     Please note there is a limit to the number of customers that can be imported in Bookeo. Bookeo is primarily a booking system, not a CRM.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customers-post-openapi.md
- name: Bookeo - Retrieve a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-get
  description: Retrieve a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-get-openapi.md
- name: Bookeo - Update the details of a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-put
  description: Update the details of a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-put-openapi.md
- name: Bookeo - Delete a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-delete
  description: Delete a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-delete-openapi.md
- name: Bookeo - Retrieve a customer
  x-api-slug: customersid-get
  description: Retrieve a customer by its id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersid-get-openapi.md
- name: Bookeo - Update an existing customer
  x-api-slug: customersid-put
  description: Update an existing customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersid-put-openapi.md
- name: Bookeo - Delete a customer
  x-api-slug: customersid-delete
  description: |-
    Delete a customer.
     Please note it is not possible to delete customers that have bookings in the future, and that are not cancelled.
     If your application needs to delete a customer with future bookings, make sure to cancel all future bookings for that customer first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersid-delete-openapi.md
- name: Bookeo - Check a customer's password
  x-api-slug: customersidauthenticate-get
  description: |-
    The customer's email address is the "username" used by Bookeo to authenticate customers.
     So to authenticate a customer your application would typically use GET /customers to search for customers with a given email address, and then GET /customers/{id}/authenticate to authenticate.
     Remember that there may be duplicate customer records with the same email address, ex. due to duplicate importing or manual record creation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersidauthenticate-get-openapi.md
- name: Bookeo - Retrieve a customer's bookings
  x-api-slug: customersidbookings-get
  description: Retrieve a customer's bookings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersidbookings-get-openapi.md
- name: Bookeo - Get the people linked to a customer
  x-api-slug: customersidlinkedpeople-get
  description: Get the people linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customersidlinkedpeople-get-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Retrieve a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-get
  description: Retrieve a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-get-openapi.md
- name: Bookeo - Update the details of a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-put
  description: Update the details of a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-put-openapi.md
- name: Bookeo - Delete a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-delete
  description: Delete a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-delete-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Retrieve a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-get
  description: Retrieve a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-get-openapi.md
- name: Bookeo - Update the details of a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-put
  description: Update the details of a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-put-openapi.md
- name: Bookeo - Delete a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-delete
  description: Delete a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-delete-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Delete a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-delete
  description: Delete a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-delete-openapi.md
- name: Bookeo - Delete a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-delete
  description: Delete a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-delete-openapi.md
- name: Bookeo - Update the details of a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-put
  description: Update the details of a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-put-openapi.md
- name: Bookeo - Update the details of a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-put
  description: Update the details of a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-put-openapi.md
- name: Bookeo - Retrieve a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-get
  description: Retrieve a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-get-openapi.md
- name: Bookeo - Retrieve a person linked to a customer
  x-api-slug: customerscustomeridlinkedpeopleid-get
  description: Retrieve a person linked to a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/customers/master/_listings/bookeo/customerscustomeridlinkedpeopleid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bmc.software.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bookeo.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bookeo
- type: x-developer
  url: https://www.bookeo.com/api/
- type: x-documentation
  url: https://www.bookeo.com/apiref/index.html
- type: x-partners
  url: https://www.bookeo.com/affiliate/
- type: x-privacy-policy
  url: https://www.bookeo.com/privacy/
- type: x-terms-of-service
  url: https://www.bookeo.com/termsofservice/
- type: x-twitter
  url: https://twitter.com/bookeo
- type: x-webhook
  url: https://www.bookeo.com/api/webhooks/
- type: x-website
  url: https://www.bookeo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---