---
layout: default
title:  "Search Page"
nav_order: 5
parent: "Information Design Templates"
---

# Search Page

The search page and search results page features a search form and some configurable filters. The filters are 
hidden by default. 

<div class="example">
  <div class="example-header">
    <div class="example-title">
      <input type="text" class="example-input">
      <button class="example-button">Search</button>
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

## Filtering

Filtering is set up by specifying one or several Tag Groups and Categories in the [product configuration](../configuration/search.md). Each Tag Group will show up as a set of filters with the Tag Group name as the label {% include example-reference.html number="2" %} and all belonging tags as options. A Categories set will show up under the label "Categories" with all configured categories as options. Each set will have the option "all" pre selected in the UI.

Toggling one or several options in a filter set will update the content item list {% include example-reference.html number="3" %} to only contain items related to the selected options. This will untoggle the "all" option of the corresponding filter set. Toggling the "all" option again will effectively untoggle all selected filters of that set.

Users may combine filters. Filters within a set combines with an OR clause. Sets are then combined with AND. This means you are able to create filter combinations like `(Theme A OR Theme B) AND (Region X OR Region Y)`.

## Search Results

The search result will feature Content Items matching the query and any applied filters. If any filters are applied the filters UI will be shown (as opposed to hidden) in the header on the result page.
