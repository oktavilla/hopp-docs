---
group: "data-models"
layout: default
title:  "Curated Content List"
nav_order: 50
parent: "Data Models"
---

# Curated Content List

{% include wip.md %}

A Curated Content List has a name and an approximate break off limit. The break off gives the editor a hint of how many teasers will be presented. The actual number of teasers presented can be affected by one or several positions being taken by ads or other Teasers. See the [configuration options for Curated Pages](../configuration/index.md#curated-page-configuration) for more info on that.

Each list is configured to, either manually or automatically, show Content Item Teasers.

{% include fields-table.md definition="content-list" parent_definition="configuration-content-list" %}

* Defined by the product [configuration](../configuration/index.md#content-lists).

A list may have automation rules. If an automated list have "Allow Manual Entries" enabled the editor may also manually populate the list with teasers. Manually placed teasers takes up positions in the beginning of the list.
