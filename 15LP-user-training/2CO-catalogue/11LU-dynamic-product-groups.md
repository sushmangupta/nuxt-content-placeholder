---
title: "Dynamic Product Groups"
slug: "dynamic-product-groups"
description: ""
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Dynamic Product Groups

Dynamic Product Groups offer a powerful way to categorize products based on specific rules tied to product attributes. This feature is particularly useful as your product catalog evolves—whether you’re adding new products, removing old ones, or making changes to existing items. The beauty of Dynamic Product Groups lies in their automatic nature: once you define the rules, the group continually updates itself according to those rules, ensuring that the relevant products are always presented as defined.

## Understanding Dynamic Product Groups

Dynamic Product Groups can be as simple or as complex as you need them to be. For instance, a basic group might include all products within a specific price range. On the other hand, a more intricate group could consist of products from selected categories, each with a specific stock range, that have been reduced in price by at least 10% and maintain an average customer rating of at least 4 stars. The flexibility of this feature means that the possibilities are virtually endless.

These dynamic groups can be used in various ways across your storefront. They can be featured on landing pages, integrated into product pages, or even serve as the content for dedicated product listing pages.

## Creating a Dynamic Product Group: A Step-by-Step Guide

Let’s walk through the process of creating a dynamic product group with a practical example. Our goal is to create a category called **Accessory Deals**, which will include all accessories priced under 10€.

1. **Navigate to the Dynamic Product Groups Section**:
    - Start by heading to **Catalogues → Dynamic Product Groups**.
2. **Create a New Dynamic Product Group**:
    - Since no groups have been created yet, click on **Add dynamic product group**.
    - In the new view, name the group **Cheap Accessories**. This name is for internal use and will not be visible to customers. Although adding a description is optional, it can be helpful for future reference.
3. **Set the Conditions**:
    - The structure for setting conditions in Dynamic Product Groups follows a simple pattern:
        - **Field**: Select the attribute you want to base the condition on.
        - **Operator**: Choose an operator, which varies depending on the selected field.
        - **Value**: Input the value that the field should be compared to.
    - Conditions can be combined using **AND** (both conditions must be met) or **OR** (at least one condition must be met). For more complex scenarios, you can stack conditions in containers across different levels.
4. **Defining Our Specific Conditions**:
    - Let’s define the conditions for our group:
        - First, set the **Field** to **Categories**.
        - Then, choose the **Operator** as **is equal to**.
        - Finally, set the **Value** to **Accessories**.
    - Click **Add AND condition** to define the next rule:
        - Select **Price** as the field, choose **is less than/equal to** as the operator, and enter **10** as the value.
    - Now, the condition reads: This dynamic product group will include all products where the category is **Accessories** and the price is less than or equal to 10€.
5. **Preview and Save**:
    - Click **Preview** to inspect the results. If everything is set up correctly, you should see one product listed—**Strings for 8€**.
    - Feel free to experiment with the conditions to see how the group changes. The interface is designed to be intuitive and user-friendly.
    - Once satisfied with the setup, click **Save** to finalize the dynamic product group.

## Assigning the Dynamic Product Group to a Category

While the dynamic group is now created, it still needs to be assigned to a category.

1. **Create a New Category**:
    - Navigate to **Catalogues → Categories**.
    - Create a new subcategory under **Accessories** and name it **Accessory Deals**.
    - Enter the category details and ensure that you activate it.
2. **Assign the Dynamic Product Group**:
    - Go to the **Product** tab within the category settings.
    - Set the **Type** to **Dynamic product group**.
    - Select the group you just created, **Cheap Accessories**.
    - Save the category.
3. **Inspect the Result**:
    - Check your storefront to ensure that the new **Accessory Deals** category displays correctly, showing the 8€ strings as expected.

One of the key benefits of Dynamic Product Groups is that they update automatically. If you later change the price of any accessory to 10€ or less, or if you add new products that meet the criteria, they will automatically be included in the **Accessory Deals** category without any further action needed on your part. This ensures your product listings are always accurate and up-to-date.
