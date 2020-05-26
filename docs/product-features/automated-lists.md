---
group: "product-features"
title:  "Automated Lists"
parent: "Features"
---

# Automated Lists

Automated lists are used for promoting related content and to automatically show most recent content, most popular content etc. Lists are defined in [the Product Configuration](../configuration/curated-content-list#automated-content-list).

## Excludes

When used in a recirculation context the list will be provided with the Content Item ID for exclusion.

## Selection Rules

Explicit Selection Rules like In category or Has Tag are used to pinpoint content of a specific kind. 
More than one rule of each type may exist. In these cases they are combined with OR. 

Relational selection rules like Same Tag or Same Brand etc only takes effect in contexts where the content either has or is a tag, category or brand. The list is in these cases provided with that meta data and it can use theat as a basis for selection. 

Relational selection rules can be combined with Explicit Selection Rules.

## Similarity 

Relational selection rules are combined with AND. Each matching Content Item will get a Similarity Score that can be used for orderering. The relation will get 1 similarity point per matching meta data. So the maximum score if all rules are applied is (number of current Content Item Tags + number of current Content Item Brands + 1). 

## Cutoffs

Cutoffs like Maximum Age or Similarity Threshold can be used to exclude irrelevant content. 

## Order

The order is applied after the selection. If the order should heed the Similarity Score the result will first be ordered by similarity and then by the selected order.

## Example

```
  {
    'same-tag': true,
    'same-category': true,
    'has-tag': ['dogs'],
    'maximum-age': 365,
    'heed-similarity-score': true,
    'order': 'recency'
  }

```

Let's say we have a content item with the following meta data:
* Tags: `sweden`, `cats`, `stockholm`
* Category: `news`

When finding content for a list based on the definition above and this particular Content Item we would then:

1. Find all articles in category `news` that are tagged with `dogs` and at least one of the tags `sweden`, 
`cats` or `stockholm`.
2. Remove any Content Item older than 365 days
3. Order by similarity
