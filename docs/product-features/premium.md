---
group: "product-features"
title:  "Premium Content/Paywall"
parent: "Features"
---

# Premium Content

There’s a [general Content Paywall setting](../configuration/general-product-preferences.md) for each product. The paywall can "disabled" or run a “free model” or “premium model”. This setting determines the current default paywall behavior for the product. The general paywall setting can be [overridden on specific articles](../data-models/content-item.md#premium) by flagging them as “always premium” or “always free”. Premium content is available for search engines at all times, regardless of paywall setting. 

## Paywall Models

### Disabled
This means the product does not require login/access for any content.

### Free Model
This means content is free by default but some Content Items may require Premium Access.

### Premium Model
This means all content is premium but some Content Items may be accessible by all.

## Paywall Behavior

The editorial platform will follow this decision tree:

<img src="https://docs.google.com/drawings/d/e/2PACX-1vSbCFZV_BVjn6oeDOL2Fo9C1Wu0OXMnI2DwOpNIjFe2oaDyHQmuDIjBuBolz-hwkl8VDpzpbbD3WE75/pub?w=908&amp;h=837">

So there are two “versions” of the paywall.  
A. With sign in  
B. Without sign in
