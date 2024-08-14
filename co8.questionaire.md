---
questions:
# 1st question
  - question: "Which templating engine is used for customizing Shopware storefront?"
    answers:
    - "Twig"
    - "Smarty"
    - "Custom"
    - "Javascript"
    correct: twig

# 2nd question
  - question: "What is the process for integrating custom Twig templates into a Shopware theme?"
    answers:
    - "Override default templates in your custom theme directory"
    - "Use Shopware's template inheritance to extend or replace default templates"
    - "Modify core Shopware Twig templates directly"
    correct: "Override default templates in your custom theme directory"

# 3rd question
  - question: "TekUniverse is planning to enhance their e-commerce site's branding by adding a custom company logo to the header. They want the logo to appear on every page, alongside the site's name. Which of the following steps should TekUniverse follow to ensure the logo appears correctly in the header across all pages?"
    answers:
    - "Modify the header.html.twig file directly in the src/Storefront/Resources/Views/storefront/page/checkout/cart directory."
    - "Add the custom logo directly to the header.html.twig file of the default Shopware theme without creating a new theme."
    - "Create a custom theme, extend the default theme, and override the header.html.twig file in the custom theme directory to include the logo."
    - "Use the Shopware admin panel to upload the logo as a media file and manually adjust its placement on each page."
    correct: ""Create a custom theme, extend the default theme, and override the header.html.twig file in the custom theme directory to include the logo."

# 4th question
  - question: "After integrating the custom logo into the header, TekUniverse needs to ensure it functions correctly on various devices. What is the appropriate step to take after deploying the new theme to confirm the logo appears correctly?"
    answers:
    - "Test the site across different devices and screen sizes to ensure the logo’s appearance is consistent and does not interfere with other header elements."
    - "Review the logo placement on the admin panel and make adjustments manually for each device."
    - "Request the client’s feedback and make adjustments based on their preferences without further testing."
    - "Only test the site on a desktop computer and assume the logo will appear correctly on other devices."
    correct: "Test the site across different devices and screen sizes to ensure the logo’s appearance is consistent and does not interfere with other header elements."

# 5th question
  - question: "What directory should TekUniverse create for their custom theme to ensure it extends the default Shopware theme?"
    answers:
    - "custom/plugins/StyleCoveTheme"
    - "src/Storefront/Resources/views/storefront/themes"
    - "public/assets/themes/StyleCoveTheme"
    - "config/themes/StyleCoveTheme"
    correct: "custom/plugins/StyleCoveTheme"
---