---
title: "Plugin base structure"
slug: "plugin-base-structure"
description: "Learning unit about basic plugin structure"
icon: ""
authors: ["Micha Hobert"]
visibility: "public"
---

# Learning Objectives

By the end of this unit, you will be able to:

- Know where to add app configurations
- Understand the basic structure and file type of app configurations

# Introduction

In this learning unit, you will learn how to add app configurations. This will save you time and add default values to your app.

## Real-world example

Imagine you are developing an app for a shipping provider. Adding the shipping methods with a plugin can be cumbersome. You need to add the shipping methods manually in the Shopware backend. To make this process easier, you can add a configuration file to your plugin that contains the shipping methods. This way, the user can easily select the shipping methods in the Shopware administration.

## Adding manifest.xml to app

An app starts with a `manifest.xml` file. This file contains all the configurations for your app. It is located in the `src/Resources` directory of your app.

The basic `manifest.xml` looks like this:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/shopware/shopware/trunk/src/Core/Framework/App/Manifest/Schema/manifest-2.0.xsd">
    <meta>
        <name>ShippingApp</name>
        <label>Shipping App</label>
        <description>This app adds 2 new shipping methods</description>
        <author>shopware AG</author>
        <copyright>(c) shopware AG</copyright>
        <version>1.0.0</version>
        <license>MIT</license>
    </meta>
</manifest>
```

For an in depth explanation of the manifest.xml file, please refer to the [official Shopware documentation](https://developer.shopware.com/docs/guides/plugins/apps/).

We will not cover the whole `manifest.xml` file in this learning unit, but focus on the configuration part.

## Shipping methods

Adding shipping methods to the app configuration can be done like this:

```xml
<shipping-methods>

    <shipping-method>
        <!-- The identifier should not change after the first release -->
        <identifier>FastShippingMethod</identifier>
        <name>Fast shipping method</name>

        <delivery-time>
            <!-- Requires a new generated UUID for your new delivery time -->
            <id>c8864e36a4d84bd4a16cc31b5953431b</id>
            <name>From 1 to 2 days</name>
            <min>1</min>
            <max>2</max>
            <unit>day</unit>
        </delivery-time>
    </shipping-method>

    <shipping-method>
        <!-- The identifier should not change after the first release -->
        <identifier>CargoShippingMethod</identifier>
        <name>Cargo shipping method</name>

        <delivery-time>
            <!-- Requires a new generated UUID for your new delivery time -->
            <id>46177c36a84b418b8ae1a22028aeb1c5</id>
            <name>From 1 to 2 weeks</name>
            <min>1</min>
            <max>2</max>
            <unit>week</unit>
        </delivery-time>
    </shipping-method>

</shipping-methods>
```

:::warning
Be careful not to change your app name afterward, otherwise your shipping methods will be added again and you have to manually clean them.
:::

Great, we added 2 shipping methods that can be selected in the Shopware administration. This will make the process of adding shipping methods easier for the user.


## System configurations

# TODO: Add system configurations


## CLI commands

You do need to refresh the app after you have added the configuration. This can be done with the `app:refresh` CLI command.

Here is a list of all **app** related CLI commands:

```bash
Available commands for the "app" namespace:
  app:activate            Activates an app
  app:create              Creates an app skeleton
  app:deactivate          Deactivates an app
  app:install             Installs an app
  app:refresh             [app:update] Refreshes an app
  app:uninstall           Uninstalls an app
  app:update              Refreshes an app
  app:url-change:resolve  Resolves app url changes
  app:validate            Validates an app

```



## Quiz

1. Where is the manifest.xml file located?
    [ ] In the root directory of the app
    [x] In the `src/Resources` directory of the app
    [ ] In the `src` directory of the app
2. What is the purpose of the `theme.json` file?
   [ ] To store the theme's PHP code
   [x] To define the theme's configuration
   [ ] To store the theme's configuration