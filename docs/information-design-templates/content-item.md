---
layout: default
title:  "Content Item Page"
nav_order: 3
parent: "Information Design Templates"
---

# Content Item Page

There is one template for each [Content Variant](../data-models/content-item.md#content-variants). Exactly what fields and data that is available is defined by the [Content Type Schema](../data-models/content-item.md).

Besides content this page may also feature recirculation, [display ads](../data-models/part-ad.md), internal ads (static page teasers) and product services teasers (e.g for subscriptions).

## Context Label

A Content Item will have a "context label" above the title. The label will consist of two parts:

1. The [Category](../data-models/category.md) of the Content Item.
2. All [Tags](../data-models/tag.md) of the Content Item that belong to [Tag Groups](../data-models/tag-group.md) defined to be used for Context Labels in the [Product Configuration](../configuration/index.md#content-item-context-label-preferences).

## Sharing

Every Content Item have "share buttons". These services are supported by default:

* Facebook
* Twitter
* E-mail

## Social Media Meta Data Tags

The Content Item Templates come with dedicated social media meta data tags that guarantees great presentation on social media platforms. 
The content of these tags will be derived from the [Promotion Data](../data-models/content-item.md#promotion--indexing-data). If none, or only partial, promotion data is present the platform will use the following fallbacks:

* **Title**  
  The platform will use Promotion Title or fallback to the Content Items Title.
* **Description**  
  The platform will use Promotion Text or fallback to the Content Items Lead.
* **Image**  
  The platform will use Promotion Image or fallback to the main image of the Content Item. 
  What the main image is will vary depending on the Content Type.

## Search Engine Meta Data Tags

The Content Item Templates come with dedicated search engine meta data tags that guarantees the content will be indexed correctly and presented well in search engines. The content of these tags will be derived from the appropriate fields of the Content Item:

* **Title**  
  The platform will use the [Indexing Title](../data-models/content-item.md#promotion--indexing-data) if present. Otherwise it will fallback to the Content Items Title.
* **Description**  
  The platform will use the Content Items Lead.
* **Content Language**  
  The platform will use the Content Items Language.

## Sponsorship

When a content item has a relationship to one or several [brands](../data-models/brand.md) that is called a sponsorship. All sponsors will be shown on the content item and link to the corresponding [brand page](brand.md).

## Recirculation

TBD
