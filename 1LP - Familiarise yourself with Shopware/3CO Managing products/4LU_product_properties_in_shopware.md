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

At first, the creation of properties is not specific for one product, but instead you create a general property and then it tis assigned to one or more products.

### Product variants

Once a product has properties, you can generate variants from it which is automatically done by Shopware if you create products through the administration.

The first product is the main variant, which has implications on how the product and its variants is displayed in the store. Each variant is treated as seperate product inside Shopware, has a seperate product number and can be customized individually.

### Product media: more than images

> Product presentation!

* product images are super important for product presentation!
* prospect clients will love to see every angle of the product!
* Shopware allowes you to upload [TBD] images per product
* consider to use zoom to your product images
* consider to use 360°images of your product images

### Scale units

Shopware has the important scale units already built in, and it is used internally for different purposes.

### Using the Rule Builder with properties

* What is the rule builder
* for avarage products, enter a weight to it so you can configure shipping costs via the Rule Builder implemented into Shopware
* it gets more complex when a product has less weight then it is big: Carrier rules.
* Also this, can be applicated with the rule builder when it comes towards you have to ship a cradle of feathers which is no weight against its real measures.
* In this case, L x W x H devided by 6000 (dev by 5000 for international shipment) comes into the game.
* The rule builder can also be used with custom properties

(* Limitations: DIY products and surface calculation)