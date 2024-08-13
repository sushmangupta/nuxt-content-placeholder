---
title: ""
slug: ""
description: ""
icon: "" # svg, png? dark mode?
authors: []
visibility: "public"
---

# Customizing storefront - Shopware frontend

Now that you have your setup ready, lets meddle a little with frontends by customizing storefront ie, to achieve visual difference in your store.

Navigate to the repository > src > Storefront > Resources > Views > storefront > page > checkout > cart and there you can see twig files . For themes, [twig](https://twig.symfony.com/doc/3.x/) is used that helps in template designing.

## Scenario

Say for instance, "TekUniverse" wants to personalize its online store by adding a custom company logo to the header of their Shopware-powered e-commerce website. The logo should be visible on every page, alongside the site's name, enhancing brand visibility and providing a consistent look and feel.

**Objective:**

Integrate the company's logo into the Shopware frontend so that it appears prominently in the header across all pages.

**Steps:**

1. **Identify the Logo Placement:**
   The development team decides to place the logo in the top-left corner of the header, next to the site name. This placement will ensure maximum visibility and brand recognition.

2. **Create a Custom Theme:**
   - The development team creates a custom theme by extending the default Shopware theme.
   - A new directory for the custom theme is set up under `custom/plugins/TechWaveTheme`.

3. **Modify the Header Template:**
   - In the custom theme directory, the team overrides the `header.html.twig` file found in the default theme.
   - The code is updated to include the HTML `<img>` tag to render the company logo. This tag is inserted before the site name within the header section.

   ```twig
   {% block layout_header_logo %}
       <a href="{{ path('frontend.home.page') }}" class="header-logo">
           <img src="{{ asset('path/to/techwave-logo.png') }}" alt="{{ 'TechWave'|trans }}">
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
   - The site is tested across different devices and screen sizes to ensure the logo is displayed correctly and does not interfere with other elements.

6. **Client Review and Approval:**
   - Once the changes are deployed, the TechWave team reviews the updated site to confirm that the logo appears as expected.
   - After approval, the site goes live with the new branding.

**Outcome:**

The custom company logo is successfully integrated into the Shopware frontend. TechWave's online store now has a personalized header that reflects its brand identity, contributing to a cohesive user experience and improved brand recognition.



