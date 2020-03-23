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
      <span class="example-context-label">Category {% include example-reference.html number="1" %}</span>
    </div>
    <div class="example-context-label-part">
      <span class="example-context-label">Tag, Tag {% include example-reference.html number="2" %}</span>
    </div>
    <div class="example-context-label-part">
      <span class="example-context-label">Tag {% include example-reference.html number="2" %}</span>
    </div>
  </div>
  <div class="example-title">
    {% include example-title.html %}
  </div>
  <div class="example-body">
    {% include example-text.html %}
  </div>
</div>

{% include generic-rules/context-label.md %}

----

## Title & Lead

The title and lead on the Content Item Page will always be based on the main Title and Lead fields. 
Promotion & Indexing Data will never be used in this context.

----

## Timestamp

If a timestamp is shown on a content item is determined by preferences in the Product Configuration. 

{% include generic-rules/timestamp.md %}

----

## Sponsorship

When a content item has a relationship to one or several [brands](../data-models/brand.md) that is called a sponsorship.

<div class="example">
  <div class="example-sponsor">
    <div class="example-group-header">Sponsored by {% include example-reference.html number="1" %}</div>
    <div class="example-sponsor-brand">
      {% include example-image.html image_size="55" %}
    </div>
    <div class="example-sponsor-brand">
      {% include example-image.html image_size="55" %}
    </div>
    {% include example-reference.html number="2" fixed="true" %}
  </div>
  <div class="example-title">
    {% include example-title.html %}
  </div>
  <div class="example-body">
    {% include example-text.html %}
  </div>
</div>

* The list of sponsors will be clearly marked {% include example-reference.html number="1" %}.
* The sponsors is represented by their Brand Logos {% include example-reference.html number="2" %} and link to their [Brand Pages](brand.md).

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

{% include wip.md %}

----

## Ads

{% include wip.md %}

