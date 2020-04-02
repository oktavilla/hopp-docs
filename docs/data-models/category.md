---
group: "data-models"
layout: default
title:  "Category"
nav_order: 3
parent: "Data Models"
---

# Category

Content Categories, or just Categories for short, are used to “package” content editorially. Think of them as “buckets”. Categories are ordered in a hierarchy and content items may be placed at any level. A content item may only belong to one category.

## Fields

{% include fields-table.md definition="category-fields" parent_definition="configuration-category-fields" %}

* Defined by the product [configuration](../configuration/categories.md).

## Meta Data

| Meta Data                                         | Required | One or many |
|:--------------------------------------------------|:---------|:------------|
| [Language](content-language.md)                   | Yes      | One         |
