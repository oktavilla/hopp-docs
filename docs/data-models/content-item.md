---
layout: default
title:  "Content Item"
nav_order: 1
parent: "Data Models"
has_children: true
has_toc: false
---

# Content Item

Content items have:

| Content Field                                   | Required |
|:------------------------------------------------|:---------|
| Title                                           | Yes      |
| Lead                                            | No       |

Every Content Item may also have other fields and may allow for different Content blocks depending on the content type.

Content Types are native to the platform and they define the data schemas for different genres of content. All content, no matter which type, can (at least theoretically) contain any kind of media, but the content type determines what the **primary storytelling medium** is.

* [Article]({{ site.baseurl }}{% link docs/data-models/content-type-article.md %})
* [Static]({{ site.baseurl }}{% link docs/data-models/content-type-static.md %})

## Content Variants

The platform comes with one or several variants of every content type. The variant defines the **storytelling mode**. A content variant maps to exactly one content type and one set of information design templates (page and teasers). See respective Content Type for available variants.

## Meta Data

Meta Data is used to describe or structure the content. Content Items (except static ones) may have relationships to meta data of different different kinds. These types of relationships are possible or required:

| Meta Data                                                                    | Required | One or many |
|:-----------------------------------------------------------------------------|:---------|:------------|
| [Category]({{ site.baseurl }}{% link docs/data-models/category.md %})        | Yes      | One         |
| [Language]({{ site.baseurl }}{% link docs/data-models/content-language.md %})| Yes      | One         |
| [Tag]({{ site.baseurl }}{% link docs/data-models/tag.md %})                  | No       | Many        |
| [Brand]({{ site.baseurl }}{% link docs/data-models/brand.md %})              | No       | Many        |
| [Contributor]({{ site.baseurl }}{% link docs/data-models/contributor.md %})  | No       | Many        |

## Social Media Promotion Data

The Content Item Information Design Templates comes with dedicated social media tags that guarantees great presentation on social media platforms. The content of these tags may be defined specifically or they will default to the data already available on the content item.

Editable fields TBD.

## Teaser Data

The content variant and type determines what sort of teaser to show on start pages and in lists. For video content the platform may show a teaser with a video play button and for a long read article there may be a larger, more engaging, image in the teaser.

Editable fields TBD.
