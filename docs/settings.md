---
layout: default
title: Settings
nav_order: 7
description: "Global app settings and controls"
---

# Settings
{: .no_toc }

<details open markdown="block">
  <summary>Table of contents</summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

## Overview

The Settings page (`/app/settings`) contains global controls that apply across all offers in your store.

---

## Global Controls

### Disable All Upsell Offers

**Toggle:** "Disable all upsell offers"

When this toggle is **enabled**, every upsell and cross-sell offer is hidden from your storefront — regardless of individual offer statuses. This is a store-wide kill switch.

**Use cases:**
- Temporarily removing all offers during a major sale or promotional event where you don't want to mix messages
- Quickly disabling offers during site maintenance
- Testing your storefront without offer widgets

> **Warning:** Enabling this overrides all individual offer statuses. Active offers will not display to customers until this toggle is turned off.

When this setting is active, the **Dashboard** shows a warning banner reminding you that all offers are globally disabled, with a direct link back to Settings.

### Saving Settings

Settings use the **Save Bar** at the top of the page. Changes are not applied until you click **Save**.

---

## Widget Appearance

Widget appearance (button colors, layout, max width) is controlled per theme block in the **Theme Editor**, not from this Settings page. See [Theme Blocks](theme-blocks) for details.

---

## Per-Offer Settings

Settings specific to individual offers (title, description, discount, trigger conditions, recommendation method) are managed on each offer's edit page. See [Creating Offers](offers/create) for details.
