---
layout: default
title: Discounts
parent: Offers
nav_order: 3
description: "Configuring percentage and fixed-amount discounts on upsell offers"
---

# Discounts
{: .no_toc }

<details open markdown="block">
  <summary>Table of contents</summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

You can attach an optional discount to any offer to incentivize customers to add recommended products to their cart.

---

## Enabling a Discount

On the **Create Offer** or **Edit Offer** page, scroll to the **Discount Offer** section and toggle **"Offer a special discount with this upsell"**.

When enabled, two additional fields appear:
- **Discount Type**
- **Discount Value**

---

## Discount Types

### Percentage Discount

Reduces the price of each recommended product by a percentage.

| Setting | Value |
|---------|-------|
| Discount Type | Percentage |
| Discount Value | e.g., `10` for 10% off |

**Example:** A product normally priced at $50 becomes $45 with a 10% discount.

**Best for:** Broad discounts that scale with product price.

---

### Fixed Amount Discount

Reduces the price by a flat dollar amount.

| Setting | Value |
|---------|-------|
| Discount Type | Fixed Amount |
| Discount Value | e.g., `5` for $5 off |

**Example:** A product normally priced at $50 becomes $45 with a $5 discount.

**Best for:** Specific, easy-to-communicate savings ("$5 off").

---

## Apply Discount to Each Item *(Fixed Amount only)*

When **Discount Type** is set to **Fixed Amount**, an additional toggle appears:

> **"Apply discount to each item"**

| Toggle | Behavior |
|--------|----------|
| **Off** (default) | The fixed amount is applied once to the entire order addition |
| **On** | The fixed amount is applied to each individual item the customer adds |

**Example:** Discount value = $5, customer adds 3 recommended products.
- Toggle **off**: $5 total discount
- Toggle **on**: $15 total discount ($5 × 3 items)

---

## How Discounts Are Applied

Discounts are calculated and displayed in the offer widget on the storefront. When a customer clicks the CTA button:
1. The recommended product (or variant) is added to the cart.
2. The discount is applied at the line item level.

> **Note:** Discounts are applied via the storefront cart API. They appear as a line item discount visible to the customer during checkout.

---

## Tips for Effective Discounts

- **Start with 10–15%** for percentage discounts — enough to nudge without sacrificing too much margin.
- **Use fixed-amount discounts** for premium products where a percentage feels small.
- **Combine with Popup offers** for urgency: the popup + a time-sensitive discount creates a strong conversion signal.
- **Don't over-discount Cart Upsell offers** — customers are already committed; a small nudge (5–10%) is often enough.
- Keep discount values **visible in the offer title or description** (e.g., "Add this for 10% off today only").
