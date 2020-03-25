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

## Start Page Content Mix

{% include wip.md %}

There is a default Content Mix for the start page. 

{% include fields-table.md definition="configuration-default-content-mix" %}

---------

## Tag Content Mixes

{% include wip.md %}

It is possible to set up additional Content Mixes to replace the default content item listing
on Tag pages.

For each Content Mix the following needs to be specified:

{% include fields-table.md definition="configuration-tag-content-mix" %}

---------

## Category Content Mixes

{% include wip.md %}

It is possible to set up additional Content Mixes to replace the default content item listing
on Category pages.

For each Content Mix the following needs to be specified:

{% include fields-table.md definition="configuration-category-content-mix" %}

---------

## Recirculation Content Mix

{% include wip.md %}

Each product has one recirculation Content Mix. It works pretty much like any other Curated Content Mix. One difference is that a recirculation list will have access to the metadata for the context where it’s shown and may have selection rules that are based on relationship criterias (e.g “same section”, “similar tags”, “same content type” or “same partner”).

There is a default recirculation content mix that will be shown on all content items. 

{% include fields-table.md definition="configuration-default-content-mix" %}

---------

## Recirculation Content Mix for specific Categories

{% include wip.md %}

You may also define different mixes to be shown on Content Items in specific categories.

{% include fields-table.md definition="configuration-category-recirculation-content-mix" %}

---------

## Curated Content Lists

{% include wip.md %}

For each Curated Content List the following needs to be specified:

{% include fields-table.md definition="configuration-curated-content-list" %}

---------

## Curated Section Configuration

{% include wip.md %}

A Curated Section consists of an ordered list of containers. Each container has a finite number of positions. Each position have a content source and an optional fallback source. A source can either be a Curated Content List, an Ad Position or a Service Teaser.

---------

## Content Item Display Preferences

{% include wip.md %}

It is possible to define preferences for how Content Items should display content in various contexts. 

{% include fields-table.md definition="configuration-content-item-display-preferences-fields" %}

---------

## Content Item Teaser Preferences

It is possible to specify teaser display preferences for each Content Variant. This overrides any defaults for that specific variant. For each variant it is possible to define:

{% include fields-table.md definition="configuration-content-teaser-preferences-fields" %}

---------

## Content Item Context Label Preferences

[Context Labels](../information-design-templates/content-item.md#context-label) are used on Content Item Pages to provide context for readers. Each product may define a few preferences in relation to these:

{% include fields-table.md definition="configuration-context-labels-fields" %}

---------

## Contact

For each product you may define one or several contact addresses. These will be swhown in the footer.
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

---------

## Accounts for 3rd party integrations

{% include wip.md %}

The platform supports integrations to some 3rd party services. The product needs to provide account details for those services in order for the integrations to work.

{% include fields-table.md definition="configuration-accounts" %}
