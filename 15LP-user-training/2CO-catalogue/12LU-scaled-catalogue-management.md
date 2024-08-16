---
title: "Scaled Catalogue Management"
slug: "scaled-catalogue-management"
description: ""
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Connection to ERP / PIM

As indicated earlier, larger shops often do not manage their product catalogs directly within the Shopware administration. Instead, these businesses typically rely on a dedicated Product Information Management (PIM) system or a broader Enterprise Resource Planning (ERP) system to handle all their product data. These systems serve as the single source of truth for the catalog, with Shopware functioning primarily as a platform that utilizes this data.

In such setups, products from the PIM or ERP systems are synchronized with the Shopware system, either in real-time (on the fly) or through periodic updates. This synchronization ensures that the product information in Shopware remains accurate and consistent with the data stored in the primary system.

When changes are made directly in the Shopware Administration, these modifications might be synchronized back to the PIM or ERP system, depending on how the systems are integrated. In some cases, the Shopware Administration is extended or customized to e.g. explicitly disallow changes, preventing conflict with the data maintained in the external system.

To facilitate these integrations, there are extensions available in the Shopware Store that enable seamless connections between Shopware and well-known external systems. However, in many cases, connecting Shopware to external systems requires individualized customization by an agency, often as part of a larger eCommerce project. These extensions allow for real-time data synchronization, ensuring that the Shopware catalog is always up-to-date with the latest information from the PIM or ERP system. This is where the Shopware APIs (Application Programming Interfaces) come into play. These APIs are essential tools for exchanging data between external systems and Shopware, enabling the integration of complex business processes and ensuring data consistency across platforms.

For those interested in the technical aspects of these integrations, detailed information can be found in our [technical documentation](https://developer.shopware.com/docs/concepts/api/). Understanding how to manage a catalog within the Shopware Administration is still important, as it provides insight into how the catalog functions within Shopware, even when external systems are involved. This knowledge is crucial for effectively managing and troubleshooting the catalog, ensuring smooth operations whether you’re working within Shopware or in conjunction with external systems.

<!-- seperate LUs -->
