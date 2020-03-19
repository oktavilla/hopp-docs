---
layout: default
title:  "Filtered Category Page"
parent: "Information Design Templates"
---

# Filtered Category Page

A [standard category page](category.md) can be “replaced” with a page that allows content filtering. In this case the user interface works a bit differently.

<div class="example">
  <div class="example-header">
    <div class="example-title">
      {% include example-title.html %}
    </div>
    <div class="example-navigation">
      <div class="example-group-header">Filter content: {% include example-reference.html number="1" %}</div>
      <div class="example-navigation-group">
        <span class="example-label">Theme:</span>
        <span class="example-navigation-item example-navigation-item-with-text example-navigation-item-selected">All</span>
        <span class="example-navigation-item"></span>
        <span class="example-navigation-item"></span>
        <span class="example-navigation-item"></span>
      </div>
      <div class="example-navigation-group">
        <span class="example-label">Region: </span>
        <span class="example-navigation-item example-navigation-item-with-text example-navigation-item-selected">All</span>
        <span class="example-navigation-item"></span>
        <span class="example-navigation-item"></span>
      </div>      
      {% include example-reference.html number="2" fixed="true" %}
    </div>
  </div>
  <div class="example-body">
    <div class="example-teaser-list">
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      {% include example-teaser.html %}
      {% include example-reference.html number="3" fixed="true" %}
    </div>
  </div>
</div>

The category page will have filters instead of ordinary navigation {% include example-reference.html number="1" %}. In case the category have sub categories those will be "hidden" (as there's no navigation) but all content will be available and filterable from this page.

Filtering is set up by specifying one or several Tag Groups in the [product configuration](../configuration/index.md#categories). Each Tag Group will show up as a set of filters with the Tag Group name as the label {% include example-reference.html number="2" %} and all belonging tags as options. Each set will have the option "all" pre selected in the UI.

Toggling one or several tags in a filter set will update the content item list {% include example-reference.html number="3" %} to only contain items related to the selected tags. This will untoggle the "all" option of the corresponding filter set. Toggling the "all" option again will effectively untoggle all selected filters of that set.

Users may combine filters. Filters within a set combines with an OR clause. Sets are then combined with AND. This means you are able to create filter combinations like `(Theme A OR Theme B) AND (Region X OR Region Y)`.

