---
layout: default
title:  "Tag Page"
nav_order: 50
parent: "Information Design Templates"
---

# Tag Page

There is one page for each Tag. The content of a tag page is determined by its [type](../data-models/tag.md).

<div class="example">
  <div class="example-header">
    <div class="example-title">
      {% include example-image.html image_size="100" %}
      {% include example-title.html %} <span class="example-reference">1</span>
    </div>
    <div class="example-navigation">
      <span class="example-navigation-item"></span>
      <span class="example-navigation-item"></span>
      <span class="example-navigation-item"></span>
      <span class="example-reference">2</span>
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

* A tag will show different information based on its type <span class="example-reference">1</span>.
* If a tag has children the tag page will feature a navigation allowing the user to drill down <span class="example-reference">2</span>.
* A tag page will always list all content items placed in or below it (latest first) <span class="example-reference">3</span>. For specific needs the standard list can be “replaced” by a [curated content mix](components-and-containers-curated-content-mix.md). 
