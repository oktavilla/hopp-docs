---
group: "configuration"
layout: default
title:  "Layout"
parent: "Curated Content"
grand_parent: "Configuration"
---

# Curated Content Layout

{% include wip.md %}

A Curated Content Layout consists of an ordered list of containers. Each container has a finite number of positions. Each position have a content source and an optional fallback source. A source can either be a Curated Content List (found by key), an Ad Position or a Service Teaser.

{% include fields-table.md definition="configuration-curated-content-layout" %}


WHAT ABOUT:
* orientation?
* ad size?
* Can we make teaser styles into an options array as well?

## Container

{% include fields-table.md definition="configuration-curated-content-container" %}

### Header

An optional header for the container.

{% include fields-table.md definition="configuration-curated-content-container-header" %}

Where a **Link** is defined as:  

{% include fields-table.md definition="configuration-curated-content-container-link" %}

### Position

A position can be defined as such:

{% include fields-table.md definition="configuration-curated-content-container-position" %}

Where a **Source** is defined as: 

{% include fields-table.md definition="configuration-curated-content-container-source" %}
