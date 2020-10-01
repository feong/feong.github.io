---
title: Shopify
date: 2020-10-01 23:42:31
tags:
---

## Shopify Linker

### Shopify

[Shopify](https://www.shopify.com/) is a platform help seller sell his products online. Seller uploads products and varaints information on it.

### Shopify Linker

**Shopify Linker** is a web tool to sync product information between Shopify and PSL(Popshop.Live), includes:

- Import Shopify Products to PSL
- Sync inventory decrease back to Shopify

<!-- more -->

### The Difference of Data model

#### Shopify

![xmVA7OWdQLcoUhB](https://i.loli.net/2020/10/01/xmVA7OWdQLcoUhB.png)

- Each product has at lease one variant.
- Each entity of the product variant can be stored in a location

#### PSL

![D8W6HImeyjlVXST](https://i.loli.net/2020/10/01/D8W6HImeyjlVXST.png)

- Product can have no variant.
- There is no concept of location

### Import Shopify Products to PSL

Because there would be many locations for Shopify, we have an agreement with the seller who wants to sync products to PSL, that we only sync the variant to PSL at the location named `Popshop Live`, `popshop live`, `PopshopLive` or `popshoplive`.

**Click Shopify Beta of iOS app to start the process**
![yrFKPvAVL5Hl8TS](https://i.loli.net/2020/10/01/yrFKPvAVL5Hl8TS.png)

**Sync States**
![ozr7AeiR1BPdXCD](https://i.loli.net/2020/10/01/ozr7AeiR1BPdXCD.png)

**Sync Interaction**
![qgGNQadwstl4PeA](https://i.loli.net/2020/10/01/qgGNQadwstl4PeA.png)

### Sync inventory decrease back to Shopify

![r1vIbCMP8Od5nsA](https://i.loli.net/2020/10/01/r1vIbCMP8Od5nsA.png)

When the `Auto Sync quantity to Shopify` turned on of the store, decreased quantity will be synced to Shopify after a new order placed. For example, Store A turned on the feature, Buy B places an order of variant C with quantity equals `10`. We will sync `-10` amount to Shopify. Then Shopify will update the its amount at the location named `Popshop Live`, `popshop live`, `PopshopLive` or `popshoplive`.

#### Test Account

| Shopify Store                                           | Account        | Password          |
| ------------------------------------------------------- | -------------- | ----------------- |
| [site](https://developmentstoreof2.myshopify.com/admin) | feong@live.com | dO!VX\$Gj7disGxy0 |
