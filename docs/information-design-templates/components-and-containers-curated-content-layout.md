---
layout: default
title:  "Curated Content Layout"
parent: "Components & Containers"
grand_parent: "Information Design Templates"
---

# Curated Content Layout

Curated Content Layouts may exist on the start page, on tag and category pages and on content item pages as recirculation.

A layout consists of a set of Containers, where each Container have a Grid and a set of Items. A Container may show it's Items either as [Teasers](components-and-containers-teaser.md) or as "full" Content Items in a [Continuous Scroll mode](../product-features/continuous-scroll.md). 

## Continuous Scroll Specifics

A Container may show it's Items in "full" using lazy loading. 

* A Content Item should be lazy loaded and rendered when the "slot" is already within the viewport or when the user is about to scroll the slot into view (utilising an offset in pixels).
* When the Content Item is in "full view" in the viewport we replace the URL in order to enable sharing etc. This also triggers a Page View for analytics purposes and ads are loaded.
