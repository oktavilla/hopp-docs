---
layout: default
title:  "Subscriptions"
nav_order: 100
has_children: false
parent: "Identity"
---

# Subscriptions

A subscription represents a current or historic connection between a customer and a package (and hence products). A subscription will only last as long as the validity period of the connected package. After that a new subscription will be created if a rollover package is defined and rollovers aren't specifically prohibited. This means loyal customers will have several successive subscriptions to a package. This is a technicality and should be taken into consideration when presenting information to end users as they  most likely view this, from their perspective, as *one* ongoing subscription.

A subscription have:

* A connection to a customer
* A connection to a package
* A connection to a package that preceded the current one (if applicable)
* A start date and an end date
* It can be set to prohibit rollovers
