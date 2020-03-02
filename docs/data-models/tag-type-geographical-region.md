---
layout: default
title:  "Geographical Region"
parent: "Tag"
grand_parent: "Data Models"
---

# Geographical Region (Tag Type)

{% include wip.md %}

This type of tag is meant to represent a geographical region. 
The platform does not have any restrictions on the definition of such 
as long as it can be described in geographical bounds.

## Fields

Besides [the basic tag fields](tag.md#fields) this type of tag may also contain:

| Field                                             | Required |
|:--------------------------------------------------|:---------|
| Geographical Bounds*                              | No       |

* Lat/Lng bounds as an array, e.g:
`[{lat: -34, lng: 151}, {lat: -23, lng: 31}]`
