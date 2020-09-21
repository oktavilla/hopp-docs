---
layout: default
title:  "User Features"
nav_order: 200
parent: "Identity"
---

# User Features

## Subscription/purchase

A subscription is for a package. The subscription process is divided into several steps:

1. Make sure we have a signed in user by requesting an email address. 
  * If the user exists they will either be asked for a password (if they have one set) or receive a “magic login link” (a temporary login token) leading to the next step in the process.
  * If the user does not exist they will get an email verification email. Clicking on that link in the mail creates a new user, signs them in via a temporary token and then redirects them to the next step in the process.
2. Make sure we have all the required information about the customer. The products in the package determine what information we ask for. 
  * Missing information is required up front in a form.
  * Existing information is displayed. The user may change it if necessary.
3. Activate subscription
4. Send confirmation/welcome email

## Paywall

See description of [Premium Content](../product-features/premium.md) on the Platform.

## Sign in

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
