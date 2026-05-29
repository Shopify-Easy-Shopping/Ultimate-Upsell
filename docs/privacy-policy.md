---
layout: default
title: Privacy Policy
description: "How Ultimate Upsell & Cross Sell collects, uses, and protects your data"
---

[← Back to Home](index)

---

# Privacy Policy

**Last updated: May 30, 2026**

This Privacy Policy describes how **Ultimate Upsell & Cross Sell** ("the App", "we", "us") collects, uses, and retains data when you install and use the App on your Shopify store. By installing the App, you agree to the practices described in this policy.

* TOC
{:toc}

---

## 1. Data We Collect

### 1.1 Merchant Account Data

When you install the App, Shopify provides us with the following store information required to operate the App:

| Data | Purpose |
|------|---------|
| **Shop domain** (e.g., `yourstore.myshopify.com`) | Identifies your store in our database and scopes all data to your account |
| **Shopify access token** | Allows the App to make authenticated API calls on your behalf (e.g., fetching products, tracking orders) |
| **Shopify session data** (state, scope, expiry) | Maintains your authenticated admin session |

We do **not** collect your personal name, email, or payment information through the App installation process.

---

### 1.2 Offer Configuration Data

Data you enter when creating or editing offers is stored and associated with your shop:

- Offer names, titles, descriptions, and CTA button text
- Offer type, status, and trigger configuration
- Selected product IDs and product titles (as Shopify GraphQL IDs)
- Recommendation method and product limit settings
- Discount type, value, and per-item settings

---

### 1.3 Analytics & Event Data

The App tracks storefront interactions to measure offer performance. This data is **anonymous** — no personally identifiable information (PII) about your customers is collected or stored.

| Event | Data Recorded |
|-------|--------------|
| **Impression** | Shop domain, offer ID, timestamp |
| **Click** | Shop domain, offer ID, product ID, timestamp |
| **Conversion** | Shop domain, offer ID, product ID, order ID, revenue amount, timestamp |

For conversion events triggered by the `orders/paid` webhook, the App receives the **Shopify order ID** and **line item details** (product IDs, quantities, prices) solely to attribute revenue to an offer. No customer name, email, address, or payment information is stored.

---

### 1.4 App Settings & Billing Data

The App stores per-shop settings including:

- Global offer enable/disable state
- Current billing plan name (FREE, STARTER, GROW, ULTIMATE)
- Billing cycle start date
- Revenue generated in the current billing cycle (aggregate dollar total only)

---

### 1.5 Data We Do NOT Collect

The App does **not** collect or store:

- Customer names, email addresses, or contact information
- Customer browsing history outside of offer interactions
- Payment card details or financial information
- Passwords or authentication credentials beyond Shopify-issued access tokens
- Any data from storefronts where the App is not installed

---

## 2. How We Use Your Data

### 2.1 To Operate the App

- Authenticating your admin session and securing API requests
- Fetching product data from your store to populate offer recommendations
- Rendering offer widgets on your storefront via the App Proxy
- Attributing revenue to specific offers via order webhook events

### 2.2 To Provide Analytics

- Aggregating impression, click, and conversion counts per offer
- Calculating performance metrics (CTR, conversion rate, revenue)
- Displaying analytics in the App dashboard

### 2.3 To Enforce Billing Plan Limits

- Tracking cumulative upsell revenue within each 30-day billing cycle
- Automatically hiding offers when the plan's revenue limit is reached
- Resetting the billing cycle counter every 30 days

### 2.4 To Improve the App

Aggregated, anonymized usage patterns (e.g., which offer types convert best) may be used internally to improve App features and performance. This analysis is never tied to individual merchants or their customers.

---

## 3. Data Sharing & Third Parties

We do **not** sell, rent, or share your data with third parties for marketing or advertising purposes.

Data may be shared only in the following limited circumstances:

| Recipient | Reason |
|-----------|--------|
| **Shopify** | The App operates within the Shopify platform. Shopify processes and routes API calls and webhook events. See [Shopify's Privacy Policy](https://www.shopify.com/legal/privacy). |
| **Hosting / infrastructure providers** | The App's server and database are hosted on cloud infrastructure. Providers are bound by data processing agreements and do not have independent access to your data. |
| **Law enforcement / legal process** | If required by applicable law, court order, or regulatory obligation, we may disclose data to the extent legally required. |

---

## 4. Data Retention

### 4.1 Active Installation

While the App is installed on your store, we retain:

| Data Type | Retention Period |
|-----------|-----------------|
| Session tokens | Until the session expires or you uninstall the App |
| Offer configuration | Indefinitely while the App is installed |
| Analytics events (OfferEvent records) | Indefinitely while the App is installed |
| Aggregate offer stats (impressions, clicks, conversions, revenue) | Indefinitely while the App is installed |
| App settings and billing cycle data | Indefinitely while the App is installed |

### 4.2 After Uninstallation

When you uninstall the App, Shopify revokes the access token immediately. We will **delete all data associated with your shop** within **30 days** of receiving the `app/uninstalled` webhook, including:

- All offer configurations
- All analytics events
- All app settings and billing records
- Your Shopify session records

If you reinstall the App after this window, you will start with a clean slate.

### 4.3 Data Export Before Uninstalling

If you wish to retain a copy of your analytics data before uninstalling, we recommend exporting it from the Analytics page prior to uninstalling.

---

## 5. Merchant Rights

### 5.1 Right to Access

You may request a copy of all data we hold associated with your shop domain by contacting us at the support email below. We will provide a response within **30 days**.

### 5.2 Right to Correction

If any stored offer data or settings are inaccurate, you can correct them directly through the App's admin interface at any time. For account-level corrections (e.g., billing plan discrepancies), contact our support team.

### 5.3 Right to Deletion

You have the right to request deletion of all your data at any time, without waiting for the automatic 30-day post-uninstall purge.

To request immediate deletion:
1. Uninstall the App from your Shopify admin.
2. Contact us at the support address below with your shop domain and a deletion request.
3. We will confirm deletion within **7 business days**.

> **Note:** Deleting your data is irreversible. All offer configurations, analytics history, and settings will be permanently removed.

### 5.4 Right to Restrict Processing

If you wish to stop analytics event collection without uninstalling the App, you can use the **"Disable all upsell offers"** toggle in the [Settings](settings) page. This stops offer widgets from rendering, which prevents any new impression, click, or conversion events from being generated.

### 5.5 Right to Data Portability

You may request an export of your data in a machine-readable format (JSON or CSV). Contact us at the support address below with your shop domain and export request.

---

## 6. Security

We implement reasonable technical and organizational measures to protect your data:

- Shopify access tokens are stored encrypted at rest
- All data transmissions between the App and Shopify use HTTPS/TLS
- The App Proxy endpoints use HMAC signature verification to ensure requests originate from Shopify storefronts
- Database access is restricted to application processes only; no public database endpoints are exposed

No system is completely secure. If you believe your account has been compromised, contact us immediately.

---

## 7. Children's Privacy

The App is intended for use by Shopify merchants operating commercial stores. It is not directed at children under the age of 13, and we do not knowingly collect data from children.

---

## 8. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last updated" date at the top of this page. We encourage you to review this policy periodically. Continued use of the App after changes are posted constitutes your acceptance of the updated policy.

For material changes, we will notify merchants via a banner in the App admin.

---

## 9. Contact

If you have questions, concerns, or requests related to this Privacy Policy, please contact us:

**Email:** joomlageek.com@gmail.com
**Response time:** Within 2 business days

---

[← Back to Home](index)
