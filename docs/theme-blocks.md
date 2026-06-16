---
layout: default
title: Theme Blocks
description: "Adding the Product Offer and Cart Upsell blocks to your Shopify theme"
---

[← Back to Home](index)

---

# Theme Blocks

* TOC
{:toc}

---

## Overview

The app uses **Shopify Theme App Blocks** to render offer widgets on your storefront. Theme blocks must be manually added to your theme via the Theme Editor before any offers will appear to customers.

There are two blocks:

| Block | Offer Types Supported | Page Template |
|-------|-----------------------|---------------|
| **Product Offer** | Bundle, Popup | Product page (`product.json`) |
| **Cart Upsell** | Cart Upsell | Cart page (`cart.json`) |

> **Important:** Even if your offers are set to **Active**, they will not appear on your storefront until the corresponding theme block is installed.

---

## Adding the Product Offer Block

The Product Offer block displays Bundle and Popup offers on your product pages.

### Steps

1. From your Shopify admin, go to **Online Store → Themes**.
2. Next to your active theme, click **Customize**.
3. In the top center dropdown, select **Products → Default product** (or whichever template your products use).
4. In the left sidebar, click **Add section** or **Add block** (depending on your theme structure).
5. Search for **"Ultimate Upsell"** or scroll to find **Product Offer** under the app blocks section.
6. Click the block to add it and position it where you want offers to appear (e.g., below the product description or add-to-cart button).
7. Click **Save**.

> **Tip:** The Dashboard detects whether this block is installed. If missing, a banner will appear with a direct link to the Theme Editor.

![Add Upsell Block](./images/add-theme-block-2.png)

---

## Adding the Cart Upsell Block

The Cart Upsell block displays Cart Upsell offers on your cart page.

### Steps

1. From your Shopify admin, go to **Online Store → Themes**.
2. Next to your active theme, click **Customize**.
3. In the top center dropdown, select **Cart** (or the template that shows your cart page).
4. In the left sidebar, click **Add section** or **Add block**.
5. Search for **"Ultimate Upsell"** or scroll to find **Cart Upsell** under the app blocks section.
6. Click the block to add it and position it above or below the checkout button.
7. Click **Save**.

---

## Block Settings

Once a block is added, you can configure it directly in the Theme Editor. Click the block in the sidebar or on the canvas to see its settings.

### Product Offer Block Settings

| Setting | Options | Description |
|---------|---------|-------------|
| **Display Type** | Bundle / Popup | Choose whether to show Bundle or Popup offers from this block instance |
| **Item List Layout** | Grid / Slider | How recommended products are arranged (Bundle only) |
| **Check All Items by Default** | Yes / No | Whether all bundle items are pre-checked (Bundle only) |
| **Show Plus Icon** | Yes / No | Show the "+" separator between bundle item cards (Bundle only) |
| **Variant Display** | Separated / Grouped by product | How product variants are presented — see [Variant Display](#variant-display) |
| **Block Max Width** | 300–1400 px | Maximum width of the offer widget |
| **Button Color** | Color picker | Background color of the Add to Cart buttons |

### Cart Upsell Block Settings

| Setting | Options | Description |
|---------|---------|-------------|
| **Item List Layout** | Grid / Slider | How recommended products are arranged |
| **Variant Display** | Separated / Grouped by product | How product variants are presented — see [Variant Display](#variant-display) |
| **Block Max Width** | 300–1400 px | Maximum width of the offer widget |
| **Button Color** | Color picker | Background color of the Add to Cart buttons |

---

## Variant Display

The **Variant Display** setting controls how product variants appear inside offer widgets. It is available on both the **Product Offer** and **Cart Upsell** blocks.

### Separated items (default)

Each variant is shown as its **own individual card**.

- A product with 3 variants (e.g., Small, Medium, Large) appears as **3 separate cards**, one for each variant.
- The customer clicks the card they want and adds it directly — no dropdown required.
- Best suited for offers where you have carefully curated which specific variants to recommend.

### Grouped by product

All variants of the same product are **merged into a single card** with a variant dropdown selector.

- A product with 3 variants appears as **1 card** with a `<select>` dropdown listing all available variants.
- When the customer changes the dropdown, the displayed price updates automatically to reflect the selected variant's price (including any active discount).
- The first available variant is pre-selected by default.
- Best suited for offers where customers should be able to choose their preferred size, color, or style.

### When to use each mode

| Scenario | Recommended Mode |
|----------|-----------------|
| Recommending specific variants (e.g., only "Black L") | **Separated** |
| Recommending a product and letting customers pick their size/color | **Grouped by product** |
| Offer contains many variants and card grid looks cluttered | **Grouped by product** |
| Offer contains carefully selected single variants | **Separated** |

> **Note:** The Grouped mode respects variant availability. Unavailable variants are shown in the dropdown with "(Unavailable)" appended and cannot be added to the cart.


| Separated Items mode                                            | Grouped by Product mode |
|-----------------------------------------------------------------|-------------------------|
| ![Separated Items mode](./images/variant-display-separated.png) | ![Grouped by Product mode](./images/varitant-display-grouped.png) |

---

## Multiple Block Instances

You can add **multiple instances** of the same block to a template. For example, you could add two Product Offer blocks — one for Bundles (above the description) and one for Popups (at the bottom of the page).

Each block instance will independently query for offers matching its configured display type.

---

## Switching Themes

If you switch to a different theme, you will need to re-add the app blocks to the new theme. The Dashboard will detect that blocks are missing and show a banner with links to the Theme Editor.

---

## Troubleshooting

**Offers are not showing on my storefront**

Check the following:
1. The correct theme block is installed on the relevant template.
2. At least one offer is set to **Active**.
3. The offer's trigger conditions match the current page (e.g., a "Specific Products" offer will only show on the trigger product's page).
4. Your billing cycle revenue has not reached the plan limit. See [Billing Plans](billing).
5. The global offer disable switch is not enabled in [Settings](settings).

**The block shows but no products appear**

- For **Manual** recommendations, ensure products are selected and available in your store.
- For **AI** recommendations, ensure there are products in your store with matching tags or collections.
- Check that the recommended products are published and available for sale.

---

[← Back to Home](index)
