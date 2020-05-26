---
group: "configuration"
layout: default
title:  "Categories"
parent: "Configuration"
nav_order: 10
---

# Categories

This configuration list determines what [Categories](../data-models/category.md) should be available in the product. The actual content of the Categories (as defined in the [data model](../data-models/category.md)) are editable in the CMS. 

For specific needs certain category pages can be configured to have a "filter UI" instead of a standard sub navigation. These pages are called [Filtered Category Pages](../information-design-templates/category-filtered.md).

For each Category that should exist you need to specify:

{% include fields-table.md definition="configuration-category-fields" %}
