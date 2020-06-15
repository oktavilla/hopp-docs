---
group: "data-models"
layout: default
title:  "Content Item"
nav_order: 1
parent: "Data Models"
has_children: true
has_toc: false
---

# Content Item

## Fields

{% include fields-table.md definition="content-item-fields" %}

Every Content Item may also have other fields and may allow for different Content blocks 
depending on the content type. See below.

## Content Types

Content Types are native to the platform and they define the data schemas for different genres of content. All content, no matter which type, can (at least theoretically) contain any kind of media, but the content type determines what the **primary storytelling medium** is.

{% include sub-items-list.md parent="Content Item" %}

## Content Variants

The platform comes with one or several variants of every content type. The variant defines the **storytelling mode**. A content variant maps to exactly one content type and one set of information design templates ([page](../information-design-templates/content-item.md) and [teasers](../information-design-templates/part-teaser.md)). See respective Content Type for available variants.

## Premium

The product has a [default paywall setting](../configuration/general-product-preferences.md). But that setting can be overwritten on a per Content Item basis. A Content Item can have a premium setting that is either:

* (not set)
* Always Free
* Always Premium

## Meta Data

Meta Data is used to describe or structure the content. Content Items (except static ones) may have relationships to meta data of different different kinds. These types of relationships are possible or required:

| Meta Data                                         | Required | One or many |
|:--------------------------------------------------|:---------|:------------|
| [Category](category.md)                           | Yes      | One         |
| [Language](content-language.md)                   | Yes      | One         |
| [Tag](tag.md)                                     | No       | Many        |
| [Brand](brand.md)                                 | No       | Many        |
| [Contributor](contributor.md)                     | No       | Many        |

## Promotion & Indexing Data

All content items have the same promotion and indexing data no matter which type they are. The data will be used for teasers and internal search results as well as search engine and social media meta data tags on content pages. See the information design template specifications for [Teasers](../information-design-templates/components-and-containers-teaser.md) and [Content Item Pages](../information-design-templates/content-item.md) for more information on how this data will be used.

{% include fields-table.md definition="promotion-fields" %}

