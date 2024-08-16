---
title: "Simple mode"
slug: "simple-mode"
description: ""
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Explore advanced product definition
Let’s now delve into the intricacies of creating and managing products, which are naturally the central components of your shop. Shopware offers extensive flexibility in defining every aspect of your products and business in great detail. While this flexibility can be overwhelming at first, it’s important to start with the basics and build up from there. For instance, we initially created our first product with only minimal information. As we progress, we will explore more advanced features.

Our exploration begins with the simplified product view. This view is designed to be straightforward and is often sufficient for initial product setup. Following this, we will move on to the advanced view, which provides a comprehensive array of options and customization features. In the advanced view, you can tailor your product settings to include variants and custom options, allowing for a more detailed and specific configuration. Finally, we will examine the product listing, focusing on effective filtering and bulk editing techniques to manage your products efficiently.

To get started, navigate to **Catalogues** and then select **Products**. From there, you can customize your product view by using the button provided to tailor the display according to your needs. You can choose to show what is necessary and hide what is not, with these customizations being specific to each tab.

The advanced view presents all possible options for product management, making it ideal for users who need to access detailed configurations. Conversely, the simplified view offers a more streamlined interface, which is perfect for beginners and provides a solid foundation for managing products effectively.

## Complete product, but simplified view

Let’s open the existing product we created and add more information, keeping things simple for now. Begin by navigating to the product and ensuring that the advanced mode is disabled. To do this, click on the three stripes menu and make sure that advanced mode is turned off. This adjustment will simplify the user interface for our current task.

We’ll start with the bare minimum of information needed for the product. The title has already been set, so we move on to the manufacturer field. Here, we have the option to create a new manufacturer on the fly and add more details later. For this example, let’s add “Fender” as a new manufacturer. Note that the manufacturer field is optional; as we learned earlier, only the product name and price are required for basic setup. We will revisit manufacturer management in more detail later in this unit.

The **Product number** is calculated automatically by the system based on the shop’s number range configuration, though it can be manually overridden if necessary. For now, let’s leave it as is. Moving on to the **Description**, which utilizes a rich text editor, you can also use HTML if desired by clicking the button on the far right of the editor. For simplicity, let’s add a few lines of description or, alternatively, use the **AI Copilot** feature to generate an initial description text.

We have already set the price for the product. However, we have the option to explore **Advanced pricing** settings, where prices can be adjusted based on payment methods or customer-specific factors. We’ll cover advanced pricing in detail later. Currently, prices in other currencies are calculated automatically according to the shopware settings. If you need to adjust the price for a specific currency, you can do so by clicking on “Currency dependent pricing.” For now, there’s no need to make any adjustments.

Next, let’s set the deliverability parameters for the product. The **stock** field allows you to define the initial number of products available. Let’s set this to 10 for now. Save the changes quickly to see that the **Available stock** field is calculated automatically. This number represents the products that have been ordered but not yet shipped; once an order is shipped, the stock count will decrease accordingly. If the **clearance sale** option is activated, the product will disappear from the storefront when stock reaches zero. Otherwise, the product remains available for purchase until you reorder from the supplier. We will leave clearance sale deactivated for now.

Moving on to **Visibility & Structure**, you can determine if and where the product will be visible. Start by defining the **Sales Channel** to which the product will be associated. Ensure that the new product is visible in our **Storefront**. Sales channels will be discussed in detail in the next learning unit. You also have the option to temporarily **activate or deactivate** the product, which allows you to fine-tune its details before making it visible to customers. Using the “set visibility for selected sales channels” option, you can specify whether the product should be visible in listings, searches, or only via a direct link. For now, there is no need to disable visibility.

Define the **category** for the product, which determines where it will appear in product listings. Let’s assign the product to the “Guitar” category.

One of the most important aspects is adding **Media** to the product. You can either use existing media or add new files via drag-and-drop. Select one picture to serve as the cover image, which will be displayed in the listing. Choose any suitable picture, or navigate to “Content → Media,” click “Generate image,” and use the Copilot to create some appealing images. For this example, add three pictures to your product.

Finally, scroll to the top and switch to the **Specifications** tab. In the **Measures & Packaging** section, enter the dimensions and weight of the package:

- Width: 420 mm
- Height: 190 mm
- Length: 1450 mm
- Weight: 11.5 kg

The **Properties** and **Custom Products** sections will be covered later in this unit. In brief, **Properties** allow you to describe and filter your product using custom attributes, while **Custom Products** enable customers to personalize products using templates.

Once you’ve entered all the information, hit “Save” and then proceed to check out the product in the storefront.
