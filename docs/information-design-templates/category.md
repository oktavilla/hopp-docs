---
layout: default
title:  "Category Page"
nav_order: 5
parent: "Information Design Templates"
---

# Category Page

There is one page for each [category](../data-models/category.md). A standard category page always list all content items placed in or below it (in a sub category). For specific needs a standard category page can be “replaced” by a [filtered category page](category-filtered.md)

<div class="example">
  <div class="example-header">
    <div class="example-title">
      {% include example-title.html %} {% include example-reference.html number="1" %}
    </div>
    <div class="example-navigation">
      <span class="example-navigation-item"></span>
      <span class="example-navigation-item"></span>
      <span class="example-navigation-item"></span>
      {% include example-reference.html number="2" %}
    </div>
  </div>
  <div class="example-body">
    <div class="example-teaser-list">
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      <span class="example-reference example-reference-fixed-right">3</span>
    </div>
  </div>
</div>

* A category page will have a title {% include example-reference.html number="1" %}.
* If a category have children the category page will feature a navigation allowing the user to drill down {% include example-reference.html number="2" %}.
* A category page will always list all content items placed in the current category or one of its child categories (latest first) {% include example-reference.html number="3" %}. For specific needs the standard list can be “replaced” by a [curated content mix](components-and-containers-curated-content-mix.md). 
