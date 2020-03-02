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

## Fields

| Field                                             | Required |
|:--------------------------------------------------|:---------|
| Title                                             | Yes      |
| Text                                              | No       |

Besides these basic fields a tag may contain fields specific for its type:

* [Edition](tag-type-edition.md)
* [Geographical Region](tag-type-geographical-region.md)
* [Keyword](tag-type-keyword.md)

## Sponsoring of a tag

A tag may be sponsored by a brand. This will effectively mean that all tagged content 
items will also be sponsored. This will stay in effect until the sponsorship is removed
from the tag.

| Meta Data                                         | Required | One or many |
|:--------------------------------------------------|:---------|:------------|
| [Brand](brand.md)                                 | No       | One         |
