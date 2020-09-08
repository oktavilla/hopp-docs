---
group: "product-features"
title:  "Display Ads"
parent: "Features"
---

# Ads

Display Ads are managed through [Google Ad Manager](https://admanager.google.com/). There are a number of [Ad Positions](../configuration/ad-positions.md) that can be configured for each product. These should be reflected as "Ad Units" in the Ad Manager setup for the product.

For each page the platform will send a set of targeting key/values:

* Tags (Array of Strings)
* Sponsored (True or false)
* Premium (True or False)
* Page Type (String, see [list of possible values](../field-types/field-type-page-type.md))

The Ad Units can then be combined with relevant targeting key/values to create "Targeting Presets" in Google Ad Manager. These can be used to more conveniently set up targeting for new Line Items.
