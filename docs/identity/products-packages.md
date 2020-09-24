---
layout: default
title:  "Products & Packages"
nav_order: 100
has_children: false
parent: "Identity"
---

# Products & Packages
{: .no_toc }

1. TOC
{:toc}

## Product

A product represents a “thing” a customer could access. It could be a printed magazine, a newsletter or online premium content. It has:

* A name
* An identifier that can be used when an external system (like the editorial part of the platform) asks if a specific customer has access.
* Requirements on a customer that wants to subscribe to it. Currently we only support “must have postal address”

## Package

A package defines access to Products. A package will have:

* A public name
* A public description
* A description/list of features
* A connection to one or several Products
* A price (optional)
* A validity period (integer, optional)
* A validity period unit (days, months, years)
* A currency
* A connection to a rollover package defining what happens to subscriptions after end of validity period (can be none, same or other) (optional)
* A country requirement that sets a restriction on country of residence for customers signing up for this package (optional)
* Archived state (meaning it will be hidden from public pages and lists)

