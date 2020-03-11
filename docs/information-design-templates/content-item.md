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

## Social Media Promotion

The Content Item Templates come with dedicated social media tags that guarantees great presentation on social media platforms. 

The content of these tags may have been [specifically defined](../data-models/content-item.md#social-media-promotion-data) or they will default to the available [content item](../data-models/content-item.md) data. 

## Search Engine Promotion

The Information Design Templates are pre optimised for great visibility in search engines through speed and industry standard use of meta data and micro formats. 

## Sponsorship

When a content item has a relationship to one or several [brands](../data-models/brand.md) that is called a sponsorship. All sponsors will be shown on the content item and link to the corresponding [brand page](brand.md).

## Recirculation

TBD
