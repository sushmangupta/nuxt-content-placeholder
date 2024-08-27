---
title: ""
slug: ""
description: ""
icon: "" # svg, png? dark mode?
authors: []
visibility: "public"
goal: "The target group should understand how Shopware is using properties to generate product variants."
---

### Product properties

Products have different properties like sizes or colors, which are displayed in online stores as one product. In the physical warehouse though, there are of course multiple products.

In Shopware, this transition from selectable properties to physical products is resolved via so called variants.

The properties you create through the administration are the base for generating these variants.

You can create custom properties like fabric or anything you can think of. The same is true for the values of said properties.

At first, the creation of properties is not specific for one product but instead, you create a general property which can be assigned to one or more products.

### Product variants

Once a product has properties assigned, you can generate variants from it which is automatically done by Shopware if you create products through the administration.

The first product is the main variant, which has implications on how the product and its variants is displayed in the store. Each variant is treated as seperate product inside Shopware, has a seperate product number and can be customized individually.

### Product presentation

It is super important for the conversion rate (how many visitors you turned into actual buyers) of your online store how you present your product items. Not only a catchy title, but also a meaningful and informative description of each and every product is essential: make sure you not only take over product specifications but also define different descriptions also for product variants, if possible. Shopware offers you all of the necessary tools to achieve this behaviour - however, you are responsible for the content.

### Product media: more than images

Additionally, product media such as product images, make your trading goods more "touchable" for a prospect client: they will love to see if you make every trifle visible.

Shopware comes with a Media Library for this approach where you can upload and assign media (not only images) to your product items. Consider to upload as many as reasonable product media, including zoom functionality or even 360° images of your product.

### Scale units

Why to maintain scale units when entering products in Shopware you ask? Of course, some of your entries will never be used directly in the front page of your store to be presented to potential clients. Instead, properties like Scale Units might be utilized for the calculation of shipping prices.

Probably the weight of a product item is the easiest way to accomplish what you want to achieve. On the other hand, carriers might charge you on the basis of volumetric weight or even girth (both calculated by usage of length, width and hight) of your shipment parcel.

When entering these values to the product, you can easily instruct the Rule Builder (you will read more about it later) to compute these complex calculations for shipping cost rules.

### Limitations unlimited

Shopware is a standard software and is not supposed to apply each and every business case. However, it is highly extendable without loosing it's possibility to update via extensions (e.g. plugins or apps, you have heard about it in another lesson before). 

One way is to find a suitable extension which resolves your issue in [Shopware store](https://store.shopware.com). If you cannot find your solution, you (as a developer) can also create your own extension. In this case, please consider to make your extension available for others in Shopware Store or to place it on GitHub with the tag _shopware6-plugin_.

Here is a good example where solving of such issues with DIY products and surface calculation have been described: [https://www.shopware.com/en/news/teaching-shopware-6-time-and-spaces/](https://www.shopware.com/en/news/teaching-shopware-6-time-and-spaces/).