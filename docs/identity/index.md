---
layout: default
title:  "Identity"
nav_order: 200
has_children: true
---

# Identity - Subscriber and Lead Management
{: .no_toc }

A system for handling subscribers, members, donors and leads for an organisation. The purpose of this system is to tie the different parts of the product experience together for the customer.

1. TOC
{:toc}

## Basic Concepts

### User

A user is basically a set of log in credentials. 
* User Name (an email address, see below)
* Password (optional)
* Two-Factor Authentication

### E-mail address

An email address. Can have a state like pending, verified and maybe unreachable.

### Customer

A customer is a person who potentially will, has had or currently have a relationship to a product. A customer may have:

* A user
* One or several subscriptions
* Name & address
* E-mail address

### Administrator

An administrator is a person who has access to the system for administrative purposes. An administrator have:

* Name
* A user

### Product

A product represents a “thing” a customer could access. It could be a printed magazine, a newsletter or online premium content.

* It has an identifier that can be used when an external system asks if a specific customer has access to this offer.
* The offer defines requirements on a customer that wants to subscribe to it. Currently we only support “must have postal address”

### Package

A package defines access to Products. A package will have:

* One or several Products
* A price (optional)
* A validity period (in months) (optional)
* A rollover package after end of validity period (can be same or other) (optional)

### Subscription

A subscription is the relationship between a customer and a plan.

* A package
* A subscription has a start date
* It can be set to “do not renew”

----------

## Admin Features

### Exports

TBD

--------

## User Features

### Subscription/purchase

A subscription is for a package. The subscription process is divided into several steps:

1. Make sure we have a signed in user by requesting an email address. 
  * If the user exists they will either be asked for a password (if they have one set) or receive a “magic login link” (a temporary login token) leading to the next step in the process.
  * If the user does not exist they will get an email verification email. Clicking on that link in the mail creates a new user, signs them in via a temporary token and then redirects them to the next step in the process.
2. Make sure we have all the required information about the customer. The products in the package determine what information we ask for. 
  * Missing information is required up front in a form.
  * Existing information is displayed. The user may change it if necessary.
3. Activate subscription
4. Send confirmation/welcome email

### Paywall

See description of [Premium Content](../product-features/premium.md) on the Platform.

### Sign in

A customer can sign in to get access to products. The sign in process is divided into several steps:

1. The sign in handler may be given an “intent URL” and a product key. This determines the URL of the page the user wants to access and the product that would allow them to do so. 
2. We ask for an email address.
  * If the user exists they will either be:  
    A. Asked for a password (if they have one set)  
    B. Receive a “magic login link” (a temporary login token) if they don’t have a password set.
  * If they don’t exist they will be notified and we return to step 1.
3. After a successful login, be either means, we redirect the user to the “intent URL”.

Gotchas:
A user may not exist. 


--------

## Page Types

Keywords pointing to specific page types in Identity.

Recognised page type keywords:
* `packages_overview_page`
* `package_page`
* `signup_confirmation_page`
* `signup_password_request_page`
* `signup_checkout_form_page`
* `signup_completion_page`
* `signin_page`
* `password_reset_page`
* `profile_page`
* `profile_edit_page`
* `profile_password_change_page`



