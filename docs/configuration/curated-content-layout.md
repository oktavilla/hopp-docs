---
group: "configuration"
layout: default
title:  "Layout"
parent: "Curated Content"
grand_parent: "Configuration"
---

# Curated Content Layout

A Curated Content Layout consists of an ordered list of containers. Each container has a finite number of positions. Each position have a content source and an optional fallback source. A source can either be a Curated Content List (found by key), an Ad Position or a Service Teaser.

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

### Position

A position can be defined as such:

{% include fields-table.md definition="configuration-curated-content-container-position" %}

Where a **Source** is defined as: 

{% include fields-table.md definition="configuration-curated-content-container-source" %}

### Content List

Instead of a fixed number of positions a container can show a list of items from a dynamic content list. We currently support:

* `children`. This lists all children of the current page, either categories or tags.


## Example

``` json
[
  {
    "template": "1_col_medium",
    "positions": [
      {
        "primary_source": {
          "source_type": "content_list",
          "source_identifier": "featured"
        }
      }
    ],
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
    "content_list": "children"
  },
  {
    "template": "1_to_4_col",
    "positions": [
      {
        "primary_source": {
          "source_type": "content_list",
          "source_identifier": "news"
        }
      },
      {
        "primary_source": {
          "source_type": "content_list",
          "source_identifier": "news"
        }
      },
      {
        "primary_source": {
          "source_type": "content_list",
          "source_identifier": "news"
        }
      },
      {
        "primary_source": {
          "source_type": "ad_position",
          "source_identifier": "ad_pos_4"
        },
        "secondary_source": {
          "source_type": "content_list",
          "source_identifier": "news"
        }
      }
    ],
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
