---
group: "configuration"
layout: default
title:  "List"
parent: "Curated Content"
grand_parent: "Configuration"
---

# Curated Content List

## Manually Curated Content List

For each manually Curated Content List the following needs to be specified:

{% include fields-table.md definition="configuration-curated-content-list" %}

----

## Automated Content List

Automated lists will find Content Items based on a set of rules. 
There are both Relational Selection Rules and Explicit Selection Rules. The former only work in specific contexts like on a Content Item Page, a Tag Page etc. The latter is used to filter out specific content regardless of context. They can be used in combination. Read more about how they work in the [Automated Lists feature description](../product-features/automated-content-lists.md).

{% include fields-table.md definition="configuration-automated-content-list" %}

----

## Predefined Lists

There's one type of predefined list:

* `predefined:children`. This is a list of child items for tag or category pages. Only works in certain contexts.
