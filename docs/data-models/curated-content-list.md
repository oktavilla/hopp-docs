---
group: "data-models"
layout: default
title:  "Curated Content List"
nav_order: 60
parent: "Data Models"
---

# Curated Content List

{% include wip.md %}

A Curated Content List has a name and an approximate break off limit. The break off gives the editor a hint of how many teasers will be presented. The actual number of teasers presented can be affected by one or several positions being taken by ads, service Teasers or other Teasers. See the [configuration options for Curated Pages](../configuration/curated-content-lists.md) for more info on that.

Each list is configured to, either manually or automatically, list Content Item Teasers. If the list is automated editors will not be able to add or remove Content Items from the list manually.

{% include fields-table.md definition="content-list" parent_definition="configuration-curated-content-list" %}

* Defined by the product [configuration](../configuration/curated-content-lists.md).

A list may have automation rules. 
