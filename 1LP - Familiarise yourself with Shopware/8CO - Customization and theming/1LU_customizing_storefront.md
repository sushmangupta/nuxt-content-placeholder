---
title: "Customizing Storefront - Shopware Frontends"
slug: "customizing-storefront"
description: "This section describes personalization of your storefront by integrating custom branding elements, improving the visual consistency and overall professionalism of your online store."
icon: "" # svg, png? dark mode?
authors: []
visibility: "public"
---

# Customizing storefront - Shopware frontend

Now that your setup is ready, lets explore. We will focus on making visual changes to enhance the appearance of your store. Consider a scenario:

TekUniverse wants to personalize its online store by adding a custom company logo to the header of their Shopware-powered website. The logo should be visible on every page, enhancing brand visibility and providing a consistent look and feel.

**Objective:**

To embed TekUniverse’s logo into the Shopware frontend so it appears consistently in the header across all pages.

## Steps

1. **Identify the logo placement:**

- Locate the logo template in the Shopware repository: `src > Storefront > Resources > Views > storefront > page > storefront > layout > header > actions`.

- The `logo.html.twig` file here defines the logo’s placement. While you can't directly modify the logo in this file, you will use it as a reference.

- Refer to [twig](https://twig.symfony.com/doc/3.x/) file to help in template designing.

2. **Create custom theme:**

- Extend the default Shopware theme by creating a custom theme. Set up a new directory: custom > plugins > SwagTemplate > src > Resources > app > views/storefront.

- This directory should replicate the structure leading to logo.html.twig for customization.

3. **Modify the Template:**

- In your new file, start by extending the original logo.html.twig file using:

```text
{% sw_extends '@Storefront/storefront/layout/header/logo.html.twig' %}
```

This is simply extending the `logo.html.twig` file from the Storefront bundle. If you would leave the file like that, it wouldn't change anything, as you are currently just extending from the original file with no overrides.

- Next, override the existing block to insert your logo. See the code below. Update the block to include an HTML `<img>` tag that renders the TekUniverse logo before the site name in the header. This tag is inserted before the site name within the header section.

   ```twig
   {% block layout_header_logo %}
       <a href="{{ path('frontend.home.page') }}" class="header-logo">
           <img src="{{ asset('path/to/tekuniverse-logo.png') }}" alt="{{ 'Tekuniverse'|trans }}">
       </a>
   {% endblock %}
   ```

4. **Add CSS for Styling:**
   - Custom CSS is added to ensure the logo is displayed at the right size and aligned properly with other header elements.
   - The CSS is written in a custom stylesheet and linked to the theme.

   ```css
   .header-logo img {
       width: 150px;
       height: auto;
       margin-right: 20px;
   }
   ```

5. **Deploy and Test:**
   - The new theme is activated in the Shopware admin panel.
   - The site is to be tested across different devices and screen sizes to ensure the logo is displayed correctly and does not interfere with other elements.

6. **Client Review and Approval:**
   - Once the changes are deployed, the TekUniverse team reviews the updated site to confirm that the logo appears as expected.
   - After approval, the site goes live with the new branding.

**Outcome:**

The custom company logo is successfully integrated into the Shopware frontend. TechWave's online store now has a personalized header that reflects its brand identity, contributing to a cohesive user experience and improved brand recognition.
