---
layout: default
title:  "Configuration"
nav_order: 30
---

# Configuration
{: .no_toc }

There are a bunch of things that can be configured for a product.
These are "hard coded" and can't be changed easily.

1. TOC
{:toc}

---------

## Tag Groups

This configuration list determines what [Tag Groups](../data-models/tag-group.md) should be available in the product. The actual content of the Tag Groups (as defined in the [data model](../data-models/tag-group.md)) are editable in the CMS. 

For each Tag Group that should exist you need to specify:
{% include fields-table.md definition="configuration-tag-group-fields" %}

---------

## Categories

This configuration list determines what [Categories](../data-models/category.md) should be available in the product. The actual content of the Categories (as defined in the [data model](../data-models/category.md)) are editable in the CMS. 

For specific needs certain category pages can be configured to have a "filter UI" instead of a standard sub navigation. These pages are called [Filtered Category Pages](../information-design-templates/category-filtered.md).

For each Category that should exist you need to specify:
{% include fields-table.md definition="configuration-category-fields" %}

---------

## Curated Content Mixes

{% include wip.md %}

There is always one default [curated content mix](../data-models/curated-content-mix.md) for recirculation and one for the start page. 
These can be configured in terms of what lists and rules they should have. 

It is also possible to set up additional curated content mixes to replace the default content item listing
on tag and category pages and for recirculation on content items in specific categories.

---------

## Content Item Display Preferences

{% include wip.md %}

It is possible to define preferences for how Content Items of different [types and variants](../data-models/content-item.md) should display content in various contexts. 
Should publishing date be shown in detail, in relative terms or not at all? Should the teaser image
be shown above, below or to the right? Etc.

---------

## Content Item Context Label Preferences

[Context Labels](../information-design-templates/content-item.md#context-label) are used on Content Item Pages to provide context for readers. Each product may define a few preferences in relation to these:

{% include fields-table.md definition="configuration-context-labels-fields" %}

---------

## Contact

For each product you may define one or several contact addresses. These will be whown in the footer.
For each contact address you may specify:

{% include fields-table.md definition="configuration-contact-fields" %}

It's also is possible to pick out a number of contributors as responsible parties for an editorial product.
These contributors will be shown first on the [contributors](../information-design-templates/contributors.md) 
page and in the footer.

{% include fields-table.md definition="configuration-responsible-parties-fields" %}

---------

## Content Languages

A number of content languages can be defined for the product. This will be used to set the language on
individual content items.

{% include fields-table.md definition="configuration-content-language-fields" %}

---------

## Logo

{% include wip.md %}

It's required to specify a logo to be used in the header and throughout the product.

---------

## Footer Content

{% include wip.md %}

It is possible to define a text that will be shown in the footer.

---------

## Main Navigation

{% include wip.md %}

The navigation can be configured for a product. TBD.

---------

## Secondary Navigation

{% include wip.md %}

Shown in the footer.

