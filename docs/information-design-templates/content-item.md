---
layout: default
title:  "Content Item Page"
nav_order: 3
parent: "Information Design Templates"
---

# Content Item Page
{: .no_toc }

There is one template for each [Content Variant](../data-models/content-item.md#content-variants). Exactly what fields and data that is available is defined by the [Content Type Schema](../data-models/content-item.md).

Besides content this page may also feature recirculation, [display ads](../data-models/part-ad.md), internal ads (static page teasers) and product services teasers (e.g for subscriptions).

1. TOC
{:toc}

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
    {% include example-title.html %}
  </div>
  <div class="example-body">
    {% include example-text.html %}
  </div>
</div>

The Content Item [Category](../data-models/category.md) will always be shown as the first label <span class="example-reference">1</span> unless the current one is specifically exempt from being shown in context labels. There may also be additonal labels <span class="example-reference">2</span> showing the most relevant tags of the Content Item. Both exemptions and additional labels are defined in the [Product Configuration](../configuration/index.md#content-item-context-label-preferences).

The platform determines what tags to show in additional labels <span class="example-reference">2</span> by looking at:   
A. The list of Tag Groups defined in the Context Label Product Configuration.  
B. Available tags on the Content Item.  
C. The maximum number of labels to show as defined in the Context Label Product Configuration.  

That data will be processed in this order:
1. The platform will look at the first group in (A).
2. We look for tags on the Content Item (B) that belong to that group. 
3. If no tag is matched we try the next group in (A) and try (2) again.
4. If one or more tags match we will show a label.
5. If the maximum number of labels (C) is reached we stop.
6. If we have run though all groups in (A) we stop.
7. We try the next group in (A) and try (2) again.

This will result in 0-(C) additional labels.

----

## Title & Lead

The title and lead on the Content Item Page will always be based on the main Title and Lead fields. 
Promotion & Indexing Data will never be used in this context.

----

## Sponsorship

When a content item has a relationship to one or several [brands](../data-models/brand.md) that is called a sponsorship.

<div class="example">
  <div class="example-title">
    {% include example-title.html %}
  </div>
  <div class="example-sponsor">
    <div class="example-sponsor-header">Sponsored by <span class="example-reference">1</span></div>
    <div class="example-sponsor-brand">
      <div class="example-image example-image-60"></div>
      <span class="example-text example-text-12"></span>
      <span class="example-text example-text-5"></span>
    </div>
    <div class="example-sponsor-brand">
      <div class="example-image example-image-60"></div>
      <span class="example-text example-text-7"></span>
      <span class="example-text example-text-5"></span>
    </div>
    <span class="example-reference example-reference-fixed-right">2</span>
  </div>
  <div class="example-body">
    {% include example-text.html %}
  </div>
</div>

* The list of sponsors will be clearly marked <span class="example-reference">1</span>.
* The sponsors is represented by their Brand Names and Logos <span class="example-reference">2</span> and link to their [Brand Pages](brand.md).

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

## Recirculation

TBD
