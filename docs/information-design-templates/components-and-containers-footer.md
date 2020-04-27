---
layout: default
title:  "Footer"
parent: "Components & Containers"
grand_parent: "Information Design Templates"
---

# Footer

The footer contains of four parts displaying information that can be configured for each product.

<div class="example example-wide">
  <div class="example-row">
    <div class="example-col">
      <a href="#">Link 1</a><br>
      <a href="#">Link 2</a><br>
      <a href="#">Link 3</a><br>
      <a href="#">Link 4</a><br>
      {% include example-reference.html fixed="true" number="1" %}
    </div>
    <div class="example-col">
      <div>
        <b>Product Title</b> {% include example-reference.html number="2" %}<br>
        Recipient {% include example-reference.html number="3" %} <br>
        Some Street 23<br>
        123 45 Stockholm
      </div>
      <div>
        <a href="#">facebook.com/xyz</a> {% include example-reference.html number="4" %}
      </div>
    </div>
    <div class="example-col">
      <a href="#"><b>Person X</b>, Editor in Chief</a><br>
      <a href="#"><b>Person Y</b>, Other Role</a><br>
      <a href="#">All Contributors</a><br>
      {% include example-reference.html fixed="true" number="5" %}
    </div>
  </div>
  <div class="example-divider"></div>
  <div class="example-container">
    {% include example-text.html %} 
    {% include example-reference.html fixed="true" number="6" %}
  </div>
</div>

The first part {% include example-reference.html number="1" %} is the [footer navigation](../configuration/navigation.md). 
This is typically used for linking to legally required pages, about pages etc.

The second part consists of three different things: 
* The [product name](../configuration/general-product-preferences.md) {% include example-reference.html number="2" %}.
* The configured [contact address](../configuration/contacts.md) {% include example-reference.html number="3" %}.
* [External footer links](../configuration/navigation.md), typically used for social media pages etc {% include example-reference.html number="4" %}.

The third part will display [responsible parties](../configuration/contacts.md) and a link to [all contributors](contributors.md) {% include example-reference.html number="5" %}

The fourth and last part {% include example-reference.html number="6" %} will display an [information text](../configuration/general-product-preferences.md) if that is configured for the product. 
This is usually used for copyright information etc.
