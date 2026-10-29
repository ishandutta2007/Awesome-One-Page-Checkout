# Awesome-One-Page-Checkout

## Top One-Page Checkout Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Checkout Optimization, Express Payments & Self-Hosted Checkout Flows*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **One-Page Checkout**. These tools enable merchants to consolidate billing, shipping, and payment into a single scrollable page—reducing friction, minimizing cart abandonment, and improving conversion rates, especially on mobile.



**Examples** include Shopify One-Page Checkout, Bolt, Fast, PeachPay, Instant Checkout, Slide Checkout, Dominate, Checkout WC, OneStepCheckout, and CartPanda (the category leaders).



**Open-source emphasis**: One-Page Checkout is a domain where open-source tooling is **platform-specific and scattered**. The strongest active project is **Spree Storefront**, a production-ready Next.js headless storefront that ships with a native **one-page checkout** supporting guest/authenticated users, multi-shipment, coupons, gift cards, and Stripe/PayPal/Adyen payments under MIT license . For Sylius (Symfony ecommerce), **Mudrak One Page Checkout** provides a plugin that replaces the default multi-step checkout with a single-page experience using Symfony UX Live Components . For Magento, **OneStepCheckout** is a long-standing commercial extension with a free demo, though it is not open-source . **CheckoutWC** offers a one-page checkout mode for WooCommerce as a paid feature . No open-source project matches the integrated payment optimization and A/B testing of Bolt or Shopify's native checkout, but Spree and Mudrak provide solid foundations for custom builds.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Shopify One-Page Checkout](https://www.shopify.com/)**  

  Shopify's native checkout redesigned into a single scrollable page with pre-filled data, auto-collapsing sections for known buyers, and Shop Pay integration; available to all merchants via checkout editor settings . Supports extensibility via checkout UI extensions on Shopify Plus .



- **[Bolt](https://www.bolt.com/)**  

  One-click checkout platform offering a WooCommerce plugin (Bolt Checkout for WooCommerce) that integrates Bolt's one-click checkout and product page checkout into existing stores .



- **[Fast](https://fast.co/)**  

  **Shut down in 2022.** Fast was a one-click checkout startup that raised $125M but burned ~$10M/month against ~$600K annual revenue before running out of funds . Listed here as a cautionary tale in the category—its GitHub repository for Fast Checkout for WooCommerce remains available but the service is defunct .



- **[PeachPay](https://peachpay.com/)**  

  Checkout platform with embedded checkout SDK; known limitations include no PayPal support in embedded mode and incomplete Apple Pay/Samsung Pay coverage on certain devices . Not to be confused with Peach Payments (South African gateway).



- **[Slide Checkout](https://apps.shopify.com/slide-ai)**  

  Shopify app offering a slide-out panel for upsells, instant checkout, live search, and cart customization; free to install with a one-click "Checkout Now" button and drag-and-drop layout editor .



- **[Dominate Checkout](https://www.dominate.co/)**  

  One-page checkout overlay for ecommerce platforms; claims 38% mobile conversion lift by placing Apple Pay, Google Pay, PayPal, and Venmo above the fold and reducing checkout from 5 pages to 1 .



- **[CheckoutWC](https://www.checkoutwc.com/)**  

  WooCommerce checkout customization plugin with a "One Page Checkout" mode (Basic tier or higher) that displays all steps on a single page; includes a visual Checkout Editor with live preview .



- **[OneStepCheckout](https://www.onestepcheckout.com/)**  

  Magento-specific one-page checkout extension (since 2010); claims 20,000+ customers and $8B+ annual transactions . Features include single-page above-the-fold layout, address autocomplete, real-time price updates, and field management . **Not open-source**—commercial extension for Magento 1 and 2.



- **[CartPanda](https://cartpanda.com/)**  

  Checkout platform offering both 1-page and 3-page checkout templates; supports Shopify integration via private app, with conversion features like WhatsApp buttons, email auto-suggestion, and payment-method discounts .



## Open-Source GitHub Projects



### Headless Storefronts with Native One-Page Checkout



- **[Spree Storefront](https://github.com/spree/storefront)**  

  Production-ready, headless ecommerce storefront for Spree Commerce built with Next.js 16 and React 19 (MIT) . Ships with a **native one-page checkout** supporting guest and authenticated users, multi-shipment, coupon codes, gift cards, store credit, and **Stripe/PayPal/Adyen payments via Payment Sessions** (card data never touches the server) . Includes DTC and B2B wholesale portal support, multi-region (country/currency/language via URL segments), and Google Analytics 4 ecommerce events. **The most complete open-source one-page checkout implementation available** for headless commerce—fork and deploy or use as a reference for custom builds.



### Platform-Specific Checkout Plugins



- **[Mudrak One Page Checkout Plugin (Sylius)](https://github.com/mudrak/one-page-checkout-plugin)**  

  Open-source Sylius plugin that replaces the default multi-step checkout with a single-page experience using Symfony UX Live Components . Features real-time updates without page reloads, automatic order processing as shipping/payment selections change, and a modified state machine allowing order completion directly from cart state. Requires PHP 8.2+ and Sylius 2.0. **The cleanest open-source one-page checkout for Symfony/Sylius stacks.**



### Additional Strong Open-Source Options



- **Medusa Express Checkout Guide** — Medusa (headless commerce) provides a step-by-step guide for building an express one-page checkout storefront on top of a Medusa application; not a drop-in plugin but a documented pattern for implementing one-page checkout with Medusa's SDK .

- **Vue Storefront External Checkout** — Community plugin for Vue Storefront enabling external checkout flows (relevant for Magento-backed headless builds) . **Niche and likely dated**—verify compatibility before use.



**Frameworks for building custom systems**: For **headless commerce**, **Spree Storefront** provides a production-ready one-page checkout you can fork and customize . For **Sylius**, **Mudrak One Page Checkout** is a direct plugin install . For **Magento**, OneStepCheckout is the established commercial option , or you can implement a custom one-page flow using Magento's quote API. For **WooCommerce**, CheckoutWC's one-page mode requires a paid license . No open-source project matches Bolt's one-click network or Shopify's native checkout optimization out of the box.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- One-page checkout implementations handling payment data must comply with **PCI DSS** requirements; self-hosted solutions require careful security hardening and tokenization to avoid exposing card data.

- **Open-source one-page checkout is platform-dependent**—Spree Storefront provides a production-ready headless implementation , Mudrak serves Sylius , but Shopify and Magento ecosystems are dominated by native checkout and commercial extensions (OneStepCheckout, CheckoutWC). Fast's shutdown serves as a reminder that checkout optimization is a crowded, capital-intensive category .

- Verify license terms for commercial use; Spree Storefront uses MIT , Mudrak's plugin is open-source (Composer package) , and CheckoutWC requires a paid license for its one-page mode .



---



**Made for ecommerce merchants, checkout optimization teams, conversion rate specialists, and headless commerce developers.**  

Let's make one-page checkout more open, but with clear eyes about the payment integration and platform constraints that remain.
