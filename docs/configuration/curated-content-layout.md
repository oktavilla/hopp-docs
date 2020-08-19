---
group: "configuration"
layout: default
title:  "Layout"
parent: "Curated Content"
grand_parent: "Configuration"
---

# Curated Content Layout

A Curated Content Layout consists of an ordered list of containers. Each container has a reference to either a [curated content list](curated-content-list.md) or a [predefined list](curated-content-list.md#predefined-lists). 

{% include fields-table.md definition="configuration-curated-content-layout" %}

## Container

{% include fields-table.md definition="configuration-curated-content-container" %}

### Header

An optional header for the container.

{% include fields-table.md definition="configuration-curated-content-container-header" %}

Where a **Link** is defined as:  

{% include fields-table.md definition="configuration-curated-content-container-link" %}

### Preferences

Specific preferences that will be sent to the corresponding template.

{% include fields-table.md definition="configuration-curated-content-container-preferences" %}

Class Names is the only standardised preference. Different templates may accept other, specific, types of preferences as well.

## Example

``` json
[
  {
    "template": "1_col_medium",
    "list": "featured",
    "header": {
      "heading": "A very nice heading",
      "sub_heading": "A perfect sub heading",
      "link": {
        "text": "All the good stuff",
        "url": "/all/good/stuff"
      },
      "text": "This section contains all the best stuff we have on offer."
    },
    "preferences": {
      "class_names": ["borderedBottom", "paddedBottom", "spacedBottomGutter"]
    }
  },
  {
    "template": "1_to_4_col",
    "list": "predefined:children"
  },
  {
    "template": "1_to_4_col",
    "list": "news",
    "header": {
      "heading": "News",
    },
    "preferences": {
      "class_names": ["paddedTopBottom", "brand_15"],
    },
    "item_preferences": {
      "padded": true,
      "highlighted": true
    }
  }
]

```
