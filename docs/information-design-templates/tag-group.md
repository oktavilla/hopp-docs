---
layout: default
title:  "Tag Group Page"
nav_order: 50
parent: "Information Design Templates"
---

# Tag Group Page

A tag group page will list all its immediate decendant tags.

<div class="example">
  <div class="example-header">
    <div class="example-title">
      {% include example-image.html image_size="100" %}
      {% include example-title.html %}
      {% include example-reference.html number="1" %}
    </div>
    <div class="example-description">
      {% include example-text.html %}
    </div>
  </div>
  <div class="example-body">
    <div class="example-teaser-list">
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      {% include example-reference.html number="2" fixed="true" %}
    </div>
  </div>
</div>

* A tag group page will show name, image and description {% include example-reference.html number="1" %}. Layout of page head will depend on [tag group configuration](../configuration/tag-groups). If no image is present, head will always be rendered as "standard".
* A tag group page will always list all tags that belong to it {% include example-reference.html number="2" %}. By default the list is ordered by Tag Name, but some Tag Types have specific sort orders (i.e Edition should be sorted by Issuing Date).
