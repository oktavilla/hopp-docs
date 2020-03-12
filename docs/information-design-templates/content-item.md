---
layout: default
title:  "Content Item Page"
nav_order: 3
parent: "Information Design Templates"
---

# Content Item Page

There is one template for each [Content Variant](../data-models/content-item.md#content-variants). Exactly what fields and data that is available is defined by the [Content Type Schema](../data-models/content-item.md).

Besides content this page may also feature recirculation, [display ads](../data-models/part-ad.md), internal ads (static page teasers) and product services teasers (e.g for subscriptions).

----

## Context Label

A Content Item may have a set of "context labels" above the title. What these labels show depends on the [Product Configuration](../configuration/index.md#content-item-context-label-preferences) and the [Meta Data](../data-models/content-item.md#meta-data) of the Content Item.

<div class="example">
  <div class="example-context-label-group">
    <div class="example-context-label-part">
      <span class="example-context-label">Category <span class="example-reference">1</span></span>
    </div>
    <div class="example-context-label-part">
      <span class="example-context-label">Tag, Tag <span class="example-reference">2</span></span>
    </div>
    <div class="example-context-label-part">
      <span class="example-context-label">Tag <span class="example-reference">2</span></span>
    </div>
  </div>
  <div class="example-title">
    <span class="example-text example-text-15"></span>
    <span class="example-text example-text-7"></span>
    <span class="example-text example-text-12"></span>
  </div>
  <div class="example-body">
    <span class="example-text example-text-3"></span>
    <span class="example-text example-text-7"></span>
    <span class="example-text example-text-15"></span>
    <span class="example-text example-text-7"></span>
    <span class="example-text example-text-6"></span>
    <span class="example-text example-text-5"></span>
    <span class="example-text example-text-12"></span>
    <span class="example-text example-text-7"></span>
    <span class="example-text example-text-15"></span>
    <span class="example-text example-text-7"></span>
    <span class="example-text example-text-12"></span>
  </div>
</div>

The Content Item [Category](../data-models/category.md) will always be shown as the first label <span class="example-reference">1</span> unless the current one is specifically exempt from being shown in context labels. There may also be additonal labels <span class="example-reference">2</span> showing the most relevant tags of the Content Item. Both exemptions and additional labels are defined in the Product Configuration.

The platform determines what tags to show in an additional label <span class="example-reference">2</span> by looking at:  
A. The Tag Group(s) mapped to the label in the [Product Configuration](../configuration/index.md#content-item-context-label-preferences).  
B. Available tags on the Content Item.  

The label will only be shown if one or several tags on the Content Item (B) belong to the mapped Tag Group (A). Even if more than one Tag Group is defined for a label the platform will only show tags from one group. In this case we look for tags in the mapped groups in order. If no tags are found in the first group we move on to the second one and so on.

----

## Sharing

Every Content Item have "share buttons". These services are supported by default:

* Facebook
* Twitter
* E-mail

----

## Meta Data Tags

### Social Media

The Content Item Templates come with dedicated social media meta data tags that guarantees great presentation on social media platforms. 
The content of these tags will be derived from the [Promotion Data](../data-models/content-item.md#promotion--indexing-data). If none, or only partial, promotion data is present the platform will use the following fallbacks:

* **Title**  
  The platform will use Promotion Title or fallback to the Content Items Title.
* **Description**  
  The platform will use Promotion Text or fallback to the Content Items Lead.
* **Image**  
  The platform will use Promotion Image or fallback to the main image of the Content Item. 
  What the main image is will vary depending on the Content Type.

### Search Engines

The Content Item Templates come with dedicated search engine meta data tags that guarantees the content will be indexed correctly and presented well in search engines. The content of these tags will be derived from the appropriate fields of the Content Item:

* **Title**  
  The platform will use the [Indexing Title](../data-models/content-item.md#promotion--indexing-data) if present. Otherwise it will fallback to the Content Items Title.
* **Description**  
  The platform will use the Content Items Lead.
* **Content Language**  
  The platform will use the Content Items Language.

----

## Sponsorship

When a content item has a relationship to one or several [brands](../data-models/brand.md) that is called a sponsorship. All sponsors will be shown on the content item and link to the corresponding [brand page](brand.md).

----

## Recirculation

TBD
