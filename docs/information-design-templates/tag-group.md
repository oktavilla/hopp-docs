---
layout: default
title:  "Tag Group Page"
nav_order: 50
parent: "Information Design Templates"
---

# Tag Group Page

A tag group page will list all its tags.

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

* A tag group page will show name, image and description {% include example-reference.html number="1" %}.
* A tag group page will always list all tags thart belong to it (latest first) {% include example-reference.html number="2" %}.
