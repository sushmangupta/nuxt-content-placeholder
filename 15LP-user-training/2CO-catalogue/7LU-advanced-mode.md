---
title: "Advanced Mode"
slug: "advanced-mode"
description: ""
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Advanced view

Let’s now delve into the advanced product options within Shopware. Begin by clicking on the menu icon, often referred to as the "burger" menu, and then select "Advanced mode." This mode provides access to a broader range of options and configurations. Note that for each tab, you can customize which sections you need and which ones you prefer to skip. While we will explore all the advanced options now, we will go into further detail later on. For a comprehensive description, you can refer to [our documentation](https://docs.shopware.com/en/shopware-6-en/catalogues).

## Additions to the General Information Tab

In the **General Information** tab, an additional option is the “Highlight product” feature. Enabling **Highlight product** will add a small “Tip” flag to your product, making it stand out.

Several new fields have been added to the pricing section:

- **Tax rates** are set within the shop settings. You can input the **gross price**, and Shopware will automatically calculate the net price (and vice versa) based on the defined tax rate. If needed, this automatic calculation can be disabled by clicking the lock icon.
- The **purchase price** can be specified in both gross and net terms for internal tracking and statistics, representing the cost price from your supplier.
- The **list price** indicates the original price, showing customers how much they save if your price is lower than the list price. This will be highlighted in the storefront.
- According to EU regulations, you can also specify the **cheapest price** in the last 30 days in both gross and net terms.

Enhancements in the **Deliverability** section include:

- **Delivery time** options, based on your shop’s configuration, as well as **restock time** settings.
- You can enable **Free shipping** to remove this product from shipping cost calculations.
- Configure **minimum and maximum order quantities** and **purchase steps** (e.g., guitar picks might be ordered only in packs of 5).

In the **Visibility & Structure** tab, you can use **tags** to mark certain products, which can be utilized later in automations, similar to how categories are used. You can also define **search keywords** specifically for the product.

Additional **labeling** options include:

- **Release date**, which specifies when the product can start being ordered. The product may be visible before this date but cannot be ordered until it is reached.
- **GTIN** (Global Trade Item Number) and **EAN** (European Article Number) are visible in the store. The **Manufacturer product number** is primarily for internal use, such as for procurement.

## Additions to the Specifications Tab

In the **Specifications** tab, enhancements include:

- **Measures & Packaging** now includes unit price calculation options, useful for products like liquids (bottles) or bulk items (pallets).
- **Essential Characteristics** helps define which characteristics should be prominently displayed in the customer’s shopping cart and during checkout.

## Advanced Pricing

**Advanced pricing** is governed by rules created in the rule builder. For example, you might want to offer special prices on a customer’s birthday. You can create a rule for this and apply it to advanced pricing. While we will cover the rule builder in a later course, for now, you can select an existing rule from the dropdown, create a new one, or search for the appropriate rule if you have many. For simplicity, select the default rule **always valid**.

You can set prices, list prices, and cheapest prices in both gross and net terms, define maximum quantities for the rule, and configure currency-specific prices. For now, click **Delete pricing rule** to return to the next tab.

## Variants

**Variants** are a powerful feature based on properties, allowing you to offer different product options without creating multiple separate products. Previously, we introduced properties and assigned values, such as a guitar with a roasted maple neck. However, if you want to offer choices, such as maple or alder necks, variants simplify this process.

Instead of cloning the product for each property combination, you can use variants. To explore this:

1. Go to the **Variants** tab.
2. Note that no variants currently exist, either physical or digital.
3. Click **Generate variants** to open a new window.
4. Select the properties you want to use for creating variants, such as Body Finishes (red and white) and Neck Materials (Alder and Roasted Maple).
5. Before proceeding, you can fine-tune the variants. Click **Price surcharges / discounts** to set additional costs for specific properties (e.g., a Roasted Maple neck costs €20 more).
6. Click **Value exclusion** to exclude certain combinations. For example, exclude a combination of a red body finish with a roasted maple neck.
7. Review the variants that will be created and click **Save variants**.

After saving, you’ll see the variants in the overview. Click on a variant name, such as **Red - Roasted Maple**, to view its details. Note that most fields are inherited from the main product, but you can overwrite these settings for individual variants. You’ll also notice that the price reflects any surcharges you’ve set.

Refresh the product detail page to see the variants in action and verify that exclusions are applied correctly.

## Layout

Shopware allows you to define the look and feel of your online shop through **Shopping Experiences**. This includes customizing product page layouts. You can create different layouts for different products, ensuring each is presented optimally. Configuration options for layouts can be accessed within the product page. We will explore Shopping Experiences in detail in the next course.

## SEO

Search Engine Optimization (SEO) is crucial for increasing organic traffic and improving search engine rankings. To optimize your product page:

1. Click the **SEO** tab.
2. **Meta title**: This appears in search engine results and browser tabs. It should be concise, descriptive, and include relevant keywords.
3. **Meta description**: A brief summary (150-160 characters) of the product, designed to attract clicks by including compelling and relevant keywords.
4. **SEO keywords**: These are specific terms that users search for. Incorporate relevant keywords into your content to improve visibility.
5. **Single canonical URL for all variants**: Helps prevent duplicate content issues by consolidating ranking signals to the preferred page version.
6. **SEO URLs (per sales channel)**: Clean, descriptive URLs that include keywords, making it easier for search engines and users to understand the page content.

SEO is a complex topic, and we offer specialized training in LP17 and LP18. For now, familiarize yourself with these basic SEO settings.

## Cross Selling

**Cross-selling** encourages customers to purchase complementary products. For example, matching guitar strings or care products. Shopware allows you to manually select cross-sell products or use dynamic product groups, which will be covered later.

To manually select products:

1. Create suitable products. For example, add “Ernie Ball EB3221 Regular Slinky 10-46” for €15 and “D'Addario EXL115 11-49 Nickel Wound” for €8.
2. Navigate back to the Fender guitar’s **Cross Selling** tab.
3. Name the cross-selling section “Accessories.”
4. Select **Manual selection** and add the two guitar strings.
5. You can reorder the products as needed.
6. Click **Save** and refresh the product detail page to see the cross-sell products displayed.

## Reviews

Finally, the **Reviews** tab provides an overview of reviews for the specific product. This feature helps you understand customer feedback and can be useful for optimizing your product catalog. We will explore reviews in more detail in a later unit. For now, note that this overview helps gauge the product's context based on customer opinions.
