---
layout: default
title:  "Configuration"
nav_order: 30
---

# Configuration

There are a bunch of things that can be configured for a product.
These are "hard coded" and can't be changed easily.

## Tag Groups

What [tag groups](../data-models/tag-group.md) should be used in the product.

## Curated Content Mixes

There is always one default [curated content mix](../data-models/curated-content-mix.md) for recirculation and one for the start page. 
These can be configured in terms of what lists and rules they should have. 

It is also possible to set up additional curated content mixes to replace the default content item listing
on tag and category pages and for recirculation on content items in specific categories.

## Content Item Display Preferences

It is possible to define preferences for how Content Items of different [types and variants](../data-models/content-item.md) should display content in various contexts. 
Should publishing date be shown in detail, in relative terms or not at all? Should the teaser image
be shown above, below or to the right? Etc.

## Content Item Context Label Preferences

It is possible to define what [Tag Groups](../data-models/tag-group.md) that should be used for [Context Labels](../information-design-templates/content-item.md#context-label). 

## Logo

It's required to specify a logo to be used in the header and throughout the product.

## Contact

For each product you may define one or several contact addresses. These will be whown in the footer.
For each contact address you may specify:

| Field                                           | Required | Type     |
|:------------------------------------------------|:---------|:---------|
| Address type/name                               | No       | String   |
| Recipient                                       | No       | String   |
| Post Office Box Number                          | No       | String   |
| Postal Code                                     | No       | String   |
| Address Locality                                | No       | String   |

## Responsible parties

It is possible to define any number of responsible parties for an editorial product.
A responsbile party is defined as a role (free text) and an id of a specific contributor.
This information will be shown on the [contributors](../information-design-templates/contributors.md) page and in the footer.

## Footer Content

It is possible to define a text that will be shown in the footer.

## Main Navigation

The navigation can be configured for a product. TBD.

## Secondary Navigation

Shown in the footer.

## Language

A content language can be defined for the product. This will be used to set the language on
individual content items. 
