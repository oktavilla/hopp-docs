---
layout: default
title:  "User Features"
nav_order: 200
parent: "Identity"
---

# User Features

## Subscriptions/purchases

There are two main views for the sale of subscriptions:

* The package overview page
* A package page

The overview lists all packages that aren't archived and each package is linked to it's individual page. The subscription process starts when a user fills in their e-mail addess and clicks on submit button on the package page. The subscription process itself is divided into two main steps:

1. Make sure we have a signed in user (based on the email address provided).
  * If the user exists they will either be asked for a password (if they have one set) or receive a “magic login link” (a temporary login token) leading to the next step in the process.
  * If the user does not exist they will get an email verification email. Clicking on that link in the mail creates a new user, signs them in via a temporary token and then redirects them to the next step in the process.
2. In the final step we ask the customer to confirm the subscription purchase and provide or confirm any required information (the products in the package determine what information we ask for). 
  * Missing information is required up front in a form.
  * Any existing information for existing customers is displayed. The user may change it if necessary.

After confirmation this we activate the subscription and send a confirmation/welcome email.

## Sign in

A customer can sign in to get access to products. The sign in process is divided into several steps:

1. The sign in handler may be given an “intent URL” and a product key. This determines the URL of the page the user wants to access and the product that would allow them to do so. 
2. We ask for an email address.
  * If the user exists they will either be:  
    A. Asked for a password (if they have one set)  
    B. Receive a “magic login link” (a temporary login token) if they don’t have a password set.
  * If they don’t exist they will be notified and we return to step 1.
3. After a successful login, be either means, we redirect the user to the “intent URL”.

## Self Service

After logging in a customer can access a "self service page" where they can:

* Change name and address
* Set or change password
* See their subscription(s)
* Cancel renewal of subscriptions
