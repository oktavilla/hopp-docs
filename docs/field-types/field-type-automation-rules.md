---
group: "field-type"
title:  "Automation Rules Field"
parent: "Field Types"
---

# Automation Rules Field

{% include wip.md %}

## Excludes

When used in a recirculation context the list will be provided with the Content Item ID for exclusion.

## Relational Selection Rules

Relational selection rules only takes effect in recirculation contexts. The list is in these cases provided with the meta data of the current Content Item and can use these as a basis for selection. These rules can be combined with Explicit Selection Rules.

* Same tag (at least one tag is the same)
* Same brand (at least one brand is the same)
* Same category

These rules are combines with AND. Each matching Content Item will get a Similarity Score that can be used for orderering. The relation will get 1 similarity point per matching meta data. So the maximum score if all rules are applied is (number of current Content Item Tags + number of current Content Item Brands + 1). 

## Explicit Selection Rules

Explicit Selection Rules are used to pinpoint content of a specific kind. 
More than one rule of each type may be set up. In these cases they are combined with OR. 

* In category (Content Item must be in specific category)
* Has tag (Content Item must be have specific tag)

## Cutoffs

Cutoffs can be used to exclude irrelevant content. Optionally used in combination with ordering.

* Maximum Age (number of days since update)
* Similarity Threshold (as score)

## Order

The order is applied after the selection. There are two options in this regard.

* Heed Similarity Score
* Order (either Recency or Popularity)

If the order should heed the Similarity Score the result will first be ordered by similarity and then by the selected order.

## Example

```
  {
    'relations': {
      {
        rule: 'same-tag'
      },
      {
        rule: 'same-category'
      }
    },
    'selections': {
      {
        rule: 'has-tag',
        value: 'dogs'
      }
    },
    'cutoffs': [
      {
        rule: 'max-age',
        value: 365
      }
    ],
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


