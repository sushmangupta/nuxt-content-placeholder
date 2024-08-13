---
title: "Theme settings"
slug: "theme-settings"
description: "Learning unit about basic theme settings"
icon: ""
authors: ["Micha Hobert"]
visibility: "public"
---

# Learning Objectives

By the end of this unit, you will be able to:

- Know where to add theme settings
- Understand the basic structure of a theme configuration
- Understand the difference between plugin and theme

# Introduction

In this learning unit, you will learn how to customize your theme with settings. This will make your theme more flexible and reusable for different use cases.

## Real-world example

Imagine you are developing a theme that has a thought through design. You want to give the user the ability to change the color of the main navigation. This is a common use case for theme settings.

To achieve this, you need to add a configuration field to your theme that allows the user to select a color for the main navigation.

## Adding theme.json to theme

To add configurations to your theme, you need to create a `theme.json` file in the `src/Resources` directory of your theme. This file will contain all the configurations for your theme.

```txt
└── themes
    └── MyTheme
        ├── src
        │   ├── Resources
        │   │   └── config
        │   │       └── theme.json 
        │   └── MyTheme.php
        └── composer.json
```

The basic theme.json looks like this:

``` json
{
  "name": "SwagBasicExampleTheme",
  "author": "Shopware AG",
  "description": {
    "en-GB": "My custom theme",
  },
  "views": [
     "@Storefront",
     "@Plugins",
     "@SwagBasicExampleTheme"
  ],
  "previewMedia": "app/storefront/dist/assets/defaultThemePreview.jpg",
  "style": [
    "app/storefront/src/scss/overrides.scss",
    "@Storefront",
    "app/storefront/src/scss/base.scss"
  ],
  "script": [
    "@Storefront",
    "app/storefront/dist/storefront/js/swag-basic-example-theme.js"
  ],
  "asset": [
    "@Storefront",
    "app/storefront/src/assets"
  ],
  "configInheritance": [
    "@Storefront",
    "@OtherTheme"
    ]
}
```

For an in depth explanation of the theme.json file, please refer to the [official documentation](https://developer.shopware.com/docs/guides/themes/theme-configuration).

But here is a short overview. It mostly consists of metadata about the theme, like the name, author, description, and preview image. The `views` array defines the order in which the theme's views are loaded. The `style` and `script` arrays define the order in which the theme's styles and scripts are loaded. The `asset` array defines the order in which the theme's assets are loaded. The `configInheritance` array defines the order in which the theme's configuration is inherited.

## Input color field

The color field is a common input field type that allows the user to select a color from a color picker. To add a color field to your theme, you need to add the following code to your `theme.json` file:

```json
{
  "config": {
    "fields": {
      "sw-color-brand-primary": {
        "label": {
          "en-GB": "Primary colour",
          "de-DE": "Primär"
        },
        "type": "color",
        "value": "#399",
        "editable": true,
        "tab": "colors",
        "block": "themeColors",
        "section": "importantColors"
      }
    }
  }
}
```

Great, we can now check in our SCSS code for this value and apply it to the main navigation.

## Using the color in SCSS

To use the color in your SCSS code, you simply use them as variables. They are injected during theme compilation. Here is an example of how to use the color in your SCSS code:

```scss
.navigation {
  background-color: $sw-color-brand-primary;
}
```


## Managing the settings view

If you have more than a few configuration fields, you might want to group them and add tabs for a better overview.

This can be done with blocks, sections and tabs.

Here is an example of how to group the color field in a section:

```json
{
  "name": "Just another theme",
  "author": "Just another author",

  "config": {
    "blocks": {
      "colors": {
        "themeColors": {
          "en-GB": "Theme colours",
          "de-DE": "Theme Farben"
        }
      }
    },
    "sections": {
      "importantColors": {
        "label": {
          "en-GB": "Important colors",
          "de-DE": "Wichtige Farben"
        }
      }
    },
    "tabs": {
      "colors": {
        "label": {
          "en-GB": "Colours",
          "de-DE": "Farben"
        }
      }
    },
    "fields": {
      "sw-color-brand-primary": {
        "label": {
          "en-GB": "Primary colour",
          "de-DE": "Primär"
        },
        "type": "color",
        "value": "#399",
        "editable": true,
        "tab": "colors",
        "block": "themeColors",
        "section": "importantColors"
      }
    }
  }
}
```

## CLI commands

You do need to compile the theme after you have added the configuration. This can be done with the CLI command `theme:compile`.

Here is a list of all **theme** related CLI commands:

```bash
Available commands for the "theme" namespace:
  theme:change         Change the active theme for a sales channel
  theme:compile        Compile the theme
  theme:create         Create a new theme
  theme:dump           Dump the theme configuration
  theme:prepare-icons  Prepare the theme icons
  theme:refresh        Refresh the theme configuration
```



## Quiz

1. Can you separate the theme configuration fields into different tabs?
  [x] Yes
  [ ] No
2. What is the purpose of the `theme.json` file?
  [ ] To store the theme's PHP code
  [x] To define the theme's configuration
  [ ] To store the theme's configuration

