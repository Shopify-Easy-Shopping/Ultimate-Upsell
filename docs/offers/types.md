---
layout: default
title: Offer Types
description: "BUNDLE, POPUP, and CART UPSELL offer types explained"
---

[← Back to Offers](index) &nbsp;|&nbsp; [← Back to Home](../index)

---

# Offer Types

* TOC
{:toc}

---

The app supports three offer types. Each type targets a different point in the customer journey and is rendered by a specific theme block on your storefront.

---

## Bundle — Frequently Bought Together

**Where it appears:** Product pages (via the **Product Offer** theme block)

**How it works:**
Displays a curated list of recommended products directly on the product page, styled as a "Frequently Bought Together" section. Customers can check/uncheck items from the bundle and add all selected products to the cart at once.

**Best for:**
- Complementary products that are naturally purchased together (e.g., a camera + memory card + case)
- Increasing average order value before the customer reaches the cart

**Theme block settings available:**
- Layout: **Grid** or **Slider**
- Check all items by default: yes/no
- Max block width (300–1400 px)
- Button color

**Configuration tips:**
- Use **Manual** recommendations to hand-pick products you know pair well
- Use **AI — Similar Products** to automatically surface items in the same collections or with shared tags

---

## Popup

**Where it appears:** Product pages (via the **Product Offer** theme block)

**How it works:**
A modal popup is triggered when the customer visits a product page. The popup presents recommended products with the option to add them to the cart.

**Best for:**
- Highlighting a single high-value upsell
- Drawing attention to a limited-time offer (pair with a discount)
- Keeping the main product page layout clean

**Theme block settings available:**
- Button color

**Configuration tips:**
- Keep the recommended product list short (1–3 items) for popup offers
- Add a discount to create urgency ("Add this item for 15% off")
- Use **AI — Bestsellers** to automatically surface your most popular products

---

## Cart Upsell

**Where it appears:** Cart page (via the **Cart Upsell** theme block)

**How it works:**
Displays a horizontal or grid list of recommended products on the cart page, shown before checkout. This is a last-chance opportunity to increase the order value.

**Best for:**
- Accessories or add-ons related to items already in the cart
- Low-cost impulse items (gift wrap, extended warranty, etc.)
- Cross-selling from a different product category

**Theme block settings available:**
- Layout: **Grid** or **Slider**
- Max block width (300–1400 px)
- Button color

**Configuration tips:**
- Cart upsell offers can use **All Products** as the trigger (since it fires on the cart page, not a specific product page)
- Use **AI — Similar Products** to automatically match recommendations to the products already in the cart
- Combine with a small discount to nudge customers over the edge

---

## Choosing the Right Type

| Goal | Recommended Type |
|------|-----------------|
| Bundle complementary products together | **Bundle** |
| Interrupt and highlight a premium upsell | **Popup** |
| Last-minute add-on before checkout | **Cart Upsell** |
| Increase AOV across all product pages | **Bundle** |
| Target cart abandonment with a deal | **Cart Upsell** + discount |

---

## Theme Block Requirements

Each offer type requires a specific theme block to be installed:

| Offer Type | Required Block |
|------------|---------------|
| Bundle | Product Offer block (on product page template) |
| Popup | Product Offer block (on product page template) |
| Cart Upsell | Cart Upsell block (on cart page template) |

See [Theme Blocks](../theme-blocks) for installation instructions.

> **Important:** If the required theme block is not installed, offers of that type will never appear on your storefront, even if the offer is set to Active.

---

[← Back to Offers](index) &nbsp;|&nbsp; [← Back to Home](../index)
