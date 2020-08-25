---
group: "configuration"
layout: default
title:  "Mix"
parent: "Curated Content"
grand_parent: "Configuration"
---

# Curated Content Mixes

There are at least two different Curated Content Mixes. Each product will have a start page content mix and a recirculation content mix by default. Additonal content mixes can be set up for specific tag pages, category pages or for recirculation purposes on content items in specific categories.

A Curated Content Mix has two purposes. First it helps the editors find the Curated Content Lists that are related to a specific page or for recirculation. Secondly it's a way to map those lists to a Curated Content Layout.

Each Curated Content Mix references a number of Curated Content Lists and a Curated Content Layout. 

---------

## Start Page Content Mix

There is a default Content Mix for the start page. 

{% include fields-table.md definition="configuration-default-content-mix" %}

---------

## Recirculation Content Mix

Each product has one recirculation Content Mix. It works pretty much like any other Curated Content Mix. One difference is that a recirculation list will have access to the metadata for the context where it’s shown and may have selection rules that are based on relationship criterias (e.g “same section”, “similar tags”, “same content type” or “same partner”).

There is a default recirculation content mix that will be shown on all content items. 

{% include fields-table.md definition="configuration-default-content-mix" %}

---------

## Recirculation Content Mix for specific Categories

You may also define different mixes to be shown on Content Items in specific categories.

{% include fields-table.md definition="configuration-category-recirculation-content-mix" %}

---------

## Recirculation Mix Inside Article Content Items

You may define different mixes to be shown inside Article Content Items. The mix will be shown in a suitable position inside the article body.

{% include fields-table.md definition="configuration-category-recirculation-mix-inside-content-items" %}

---------

## Tag Content Mixes

It is possible to set up additional Content Mixes to replace the default content item listing
on Tag pages.

For each Content Mix the following needs to be specified:

{% include fields-table.md definition="configuration-tag-content-mix" %}

---------

## Category Content Mixes

It is possible to set up additional Content Mixes to replace the default content item listing
on Category pages.

For each Content Mix the following needs to be specified:

{% include fields-table.md definition="configuration-category-content-mix" %}
