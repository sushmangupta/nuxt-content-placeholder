---
title: "Custom style - Shopwrae frontends"
slug: "custom-styling"
description: "This section describes personalization of your storefront by integrating custom branding elements, improving the visual consistency and overall professionalism of your online store."
icon: "" # svg, png? dark mode?
authors: []
visibility: "public"
---

# Custom CSS

### Use Case: Customizing Product Card Layout with Custom CSS

**Scenario:**

An online fashion retailer, "TekUniverse," wants to enhance the appearance of the product cards on their Shopware store’s category pages. They want to make the product titles bold, increase the font size of the prices, and add a hover effect that slightly enlarges the product images when users hover over them.

**Objective:**

Apply custom CSS to modify the product card layout, ensuring the changes improve the visual appeal and usability of the site.

**Steps:**

1. **Identify the Target Elements:**
   - The development team identifies the specific elements within the product card that need customization:
     - Product titles: `<div class="product-name">`
     - Prices: `<span class="product-price">`
     - Product images: `<img class="product-image">`

2. **Create a Custom Theme:**
   - A custom theme, "StyleCoveTheme," is created by extending the default Shopware theme.
   - The custom theme's directory is set up under `custom/plugins/StyleCoveTheme`.

3. **Add Custom CSS:**
   - The team creates a custom stylesheet within the theme directory, typically located at `custom/plugins/StyleCoveTheme/src/Resources/views/storefront/assets/style.css`.
   - The following CSS is written to achieve the desired styling changes:

   ```css
   /* Make product titles bold */
   .product-name {
       font-weight: bold;
   }

   /* Increase font size of product prices */
   .product-price {
       font-size: 1.2rem;
       color: #ff4500; /* Optional: Change the price color to a more eye-catching shade */
   }

   /* Add a hover effect to enlarge product images */
   .product-image {
       transition: transform 0.3s ease;
   }

   .product-image:hover {
       transform: scale(1.05); /* Slightly enlarge the image on hover */
   }
   ```

4. **Integrate the Custom CSS:**
   - The custom stylesheet is linked to the theme’s `base.html.twig` or `storefront.html.twig` file to ensure it is loaded on the site:

   ```twig
   {% block base_stylesheets %}
       {{ parent() }}
       <link rel="stylesheet" href="{{ asset('custom/plugins/StyleCoveTheme/src/Resources/views/storefront/assets/style.css') }}">
   {% endblock %}
   ```

5. **Deploy and Test:**
   - The custom theme is activated, and the site is refreshed to apply the new styles.
   - The changes are tested across various devices and screen sizes to ensure the product cards are displayed correctly and that the hover effect works smoothly.

6. **Client Review and Feedback:**
   - The StyleCove team reviews the updates to the product cards and provides feedback.
   - Any necessary adjustments are made based on the client’s input before the site goes live.

**Outcome:**

The product cards on TekUniverse's category pages now feature bold titles, larger and more visually striking prices, and an interactive hover effect on images. These customizations make the product listings more engaging and user-friendly, likely contributing to better customer interaction and increased sales.
