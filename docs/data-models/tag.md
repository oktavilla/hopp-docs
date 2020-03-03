---
layout: default
title:  "Tag"
nav_order: 4
parent: "Data Models"
has_children: true
has_toc: false
---

# Tag

Tags are used to describe content but are also content in its own regard. There are a few tag types native to the platform. All these tag types have separate schemas and information design templates that define what type of content they may have and how they are displayed on articles, in lists and as a page.

A tag must belong to a [Tag Group](tag-group-md).


## Fields

{% include fields-table.md definition="tag-fields" %}

Besides these basic fields a tag may contain fields specific for its type:

* [Edition](tag-type-edition.md)
* [Geographical Region](tag-type-geographical-region.md)
* [Keyword](tag-type-keyword.md)
