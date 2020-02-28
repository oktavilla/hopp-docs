---
layout: default
title:  "Curated Content Mix"
nav_order: 50
parent: "Data Models"
---

# Curated Content Mix

** NOTE: This is WIP **

The Start Page or an Curated Sub Start Page contains an ordered set of named lists. Each list is configured to, either manually or automatically, show content item teasers. Such a set of lists, their settings and automation rules are referred to as a “curated content mix” in the platform. The list definitions and their order is set up in the product configuration. A Curated Sub Start Page can be set up to either be shown on a tag, category, partner or contributor page.

An automated list will have a number of slots as well as selection and order rules. The selection rules are basically metadata filters and the result set is ordered according to the settings and then cut of based on the number of available slots. An automated list may also be manually populated with teasers by an editor. Manually placed teasers takes up slots either in the beginning or at the end of the list depending on your configuration.

## Recirculation

Each content pool has one or several recirculation content mixes. These work very much similar to the start page and the curated section pages. One difference is that a recirculation container will have access to the metadata for the context where it’s shown and may have selection rules that are based on relationship criterias (e.g “same section”, “similar tags”, “same content type” or “same partner”).

There is a default recirculation content mix that will be shown on all content items but you may also define different mixes to be shown in specific sections.
