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
      <div class="example-image example-image-100"></div>
      {% include example-title.html %} <span class="example-reference">1</span>
    </div>
    <div class="example-description">
      {% include example-text.html %}
    </div>
  </div>
  <div class="example-body">
    <div class="example-teaser-list">
      <div class="example-teaser">
        <div class="example-image example-image-55"></div>
        {% include example-text-medium.html %}
      </div>
      <div class="example-teaser">
        <div class="example-image example-image-55"></div>
        {% include example-text-medium.html %}
      </div>
      <div class="example-teaser">
        <div class="example-image example-image-55"></div>
        {% include example-text-medium.html %}
      </div>
      <span class="example-reference example-reference-fixed-right">2</span>
    </div>
  </div>
</div>

* A tag group page will show name, image and description <span class="example-reference">1</span>.
* A tag group page will always list all tags thart belong to it (latest first) <span class="example-reference">2</span>.
