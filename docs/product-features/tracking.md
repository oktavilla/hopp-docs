---
group: "product-features"
title:  "Traffic & Behavior Tracking"
parent: "Features"
---

# Traffic & Behavior Tracking

* Page visits and Users are tracked with Google Analytics.
* We log the visits to a GA property owned by the product owner.
* We use three GA views for each product:
  * One for visits to the editorial product
  * One for visits to subscription and account managements pages
  * One that is used on both
* Visits from logged in admin users are excluded
* We store custom dimensions to allow deeper analysis

## Custom dimensions

| Custom Dimension Name | Index | Scope | Value |
| --------------------- | ----- | ----- | ----- |
| `page_type`           | 1     | Hit   | A reference to the [page type](../field-types/field-type-page-type.md) |
| `page_id`             | 2     | Hit   | The unique platform identifier for the visited page (i.e the Content Item ID) |
| `signed_in`           | 3     | Hit   | Boolean (is the visitor signed in?) |
| `subscriber`          | 4     | Hit   | Boolean (is the visitor an active subscriber?) |
