---
title: ""
slug: ""
description: ""
icon: "" # svg, png? dark mode?
authors: []
visibility: "public"
---

## Stuffing the catalog part of your online shop via administration panel

Now let's have a closer look to the question: How do products come into my online shop, what possibilities do I have?

Technically seen, the administration panel is yet another frontend. Everything entered or altered here, is stored to the database. Usually, in so called "monolithic" shopping cart systems, the application's framework is used to store data you enter into the database. This is different in Shopware as the administration panel is yet another API end-point.

BTW: When you personally get towards to the challange to write an interface between Shopware and any other system for e.g. product exchange, please use Shopware's Rest(full) API. Of course, there is also the possibility to use the framework itself but this is not recommended because of maintenance efforts: The Shopware framework may change much faster than it's API.

Depending if you are already bound to an ERP system, on the size of the product range, the frequency of orders or the number of you clients, it absolutely makes sense to use the administration panel to steer everything in your online store. If you or your client belong to the SME range of business, let's say sell ~300 products and have ten or twelve orders a day, you might be happy with this system.