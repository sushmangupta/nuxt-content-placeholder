---
title: "Getting started"
slug: "getting-started"
description: ""
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Getting started
Now that you have walked through the preparation steps and a Shopware instance available to accompany you in this journey, let's start doing.

## Goal of this learning unit
In this learning unit, we will first provide an overview of the fundamental building blocks of ecommerce. Understanding these components is crucial as they form the foundation of any online retail operation. We will then explore how these foundational elements are reflected in the Shopware Administration interface.

Then, we will cover some useful navigation and browser tips, as well as suggested settings and your setup for digest the material most effectively.

Following this, we will take a quick look at <!--internationalization, a crucial aspect for businesses aiming to reach global markets, as well as -->the possibilities for extending your Shopware installation to suite your needs best.

So, let's roll into the details and get started with the essentials of ecommerce and how they integrate with the Shopware system!

## The Building Blocks of Your Online Shop

To establish a successful online shop, it's essential to understand the fundamental components that make up your e-commerce platform.

**In a nutshell**, linking to the shopware navigation: Your products (-> **Catalogues**) are ordered (-> **Orders**) by customers (-> **Customers**). Your sales are driven by immersive shopping experience and content (-> **Content**), in a theme shining your brand (-> **Themes**). You do dedicated marketing (-> **Marketing**), and also extend (-> **Extensions**) and configure (-> **Settings**) your Shopware to suite your business requirements best!

<!--### In broader words:
Your **catalogue** is a critical aspect of any online shop. This includes managing **products**, which are the core of your catalogue, and involves detailing each item’s specifications, pricing, and availability. Managing **manufacturers** is important, as they influence the perceived value of your products. Also, **reviews** play a significant role in influencing this value, hence customer decisions and trust, so managing and displaying customer feedback is vital. In this context, **categories** help in organizing products into logical groups, making it easier for customers to navigate and find what they are looking for. **Properties** refer to the attributes of products, such as size, color, and material, which can be used to filter and sort items. Additionally, **Dynamic Product Groups** allow you to create flexible and automated collections of products based on certain criteria or rules.

The **Checkout, Orders, Payment, and Shipping** process is crucial for the operational side of your online shop. The checkout process must be streamlined and user-friendly to reduce cart abandonment and enhance customer satisfaction. Managing **Orders** involves tracking and processing purchases, handling returns, and ensuring timely fulfillment. **Payment** options must be secure and varied to accommodate different customer preferences. Finally, efficient **Shipping** management is essential for delivering products to customers in a timely manner while providing tracking and support.

**Customers** are another fundamental component. This block encompasses managing customer accounts, tracking customer interactions, and understanding purchasing behavior. Effective customer management helps in personalizing the shopping experience and fostering customer loyalty.

**Content and Marketing** are key to attracting and engaging customers. This includes creating compelling content, such as product descriptions, blog posts, and promotional materials, to drive traffic and boost sales. Marketing strategies and tools help you reach your target audience through various channels, including email campaigns, social media, and paid advertising.

**Sales Channels** represent the various platforms through which you sell your products. This could include your main website, mobile apps, social media marketplaces, or third-party platforms. Properly managing and integrating these sales channels ensures that you can reach your audience across different touchpoints and provide a consistent shopping experience.

Together, these building blocks form the foundation of a well-functioning online shop, enabling you to effectively manage products, serve customers, and drive sales. Understanding and optimizing each component will contribute to the overall success of your ecommerce venture.-->

## The Administration

Let's not dive into the Administration interface!

### Logging In

To access the Administration interface of your Shopware installation, you will need to log in through the `/admin` URL of your shop domain. Use your Shopware login credentials to enter the system. If you have forgotten your password, there is an option to reset it directly from the login page.

### Overview of the Administration Interface

The Shopware administration interface is designed to be user-friendly and intuitive. Here’s a breakdown of its main components:

- **Dashboard**: Upon logging in, you will be greeted by the dashboard, which features helpful guides and an overview of key metrics and updates.
- **Menu on the Left Side**: The main navigation menu is located on the left side of the interface. This menu is organized into several categories (from top to bottom):
    - **Navigation Items**: The menu includes items for Dashboard, Catalogues, Orders, Customers, Content, Marketing, and Settings. Hover over a menu item to view its sub-items, or click on it to expand and access additional options.
    - **Sales Channels**: Below the main navigation items, you will find a list of your sales channels.
    - **Menu Customization**: The whole menu can be minimized to save screen space.
    - **Profile**: You will also find profile settings here, where you can adjust your user interface language, update your password, and configure other personal preferences, and log out.
- **Central Search**: Located prominently, the central search function allows you to quickly locate products, categories, customers, orders, media, or other functionalities within the administration interface.
- **Notification Center**: Positioned at the top right, the notification center provides updates and alerts related to your shop’s activity, system messages, and other important information.
- **Help**: The question mark icon provides you with useful links to documentation and support. Also, you can create and copy an access link that comes in handy in the support process, letting externals enter your Administration without the hassle of sharing passwords. On the bottom, you find a link to useful keyboard shortcuts!

<!--### Familiarizing Yourself with the Administration Interface

It is important to take some time to explore and familiarize yourself with the administration interface. Understanding the layout and navigation will make it easier to manage your inventory and other shop components efficiently. The interface is designed to be self-explanatory, but getting comfortable with it will enhance your workflow.

For further guidance, refer to the following documentation resources:

- **Administration Overview**: [Shopware Administration Overview](https://docs.shopware.com/en/shopware-6-en/first-steps/administration-overview?category=shopware-6-en/getting-started)
- **Profile Settings**: [Profile Settings Documentation](https://docs.shopware.com/en/shopware-6-en/settings/Profilesettings?category=shopware-6-en/getting-started)
- **Search Functionality**: [Search Administration Guide](https://docs.shopware.com/en/shopware-6-en/first-steps/search-administration?category=shopware-6-en/getting-started)
- **Dashboard**: [Dashboard Documentation](https://docs.shopware.com/en/shopware-6-en/first-steps/dashboard?category=shopware-6-en/getting-started)-->

## Recognize the building blocks of ecommerce in your installation

Let's now identify the building blocks of eCommerce in the shopware Administration and cover the modules in a nutshell. We will get into each and every module in detail in this and the following courses!

### Catalogues: Defining Your Store

Catalogues form the core of your store, encompassing several critical elements:

- **Products**: This module allows you to view all products and add new ones. Products are fundamental to every online store, acting as the primary items that customers purchase.
- **Reviews**: Here, you can view customer reviews submitted through the storefront, offering valuable feedback and insights.
- **Categories**: This module enables you to manage the category structure of your store, which is essential for organizing your shop. Essentially, it helps structure the top and footer navigation of your shop.
- **Dynamic Product Groups**: This functionality allows you to create dynamic rules for grouping products, which in turn can be used for product listing pages or explicit landing pages with commerce components.
- **Properties**: Depending on your needs, you can define various properties for your products, such as colors, sizes, materials, ingredients, etc. This flexibility ensures that your product catalogue accurately represents your offerings.
- **Manufacturers**: This section provides an overview and the ability to create new manufacturers. Manufacturers can be crucial for how products are presented and filtered within your catalogue, allowing products to be associated with specific manufacturers.

For a more detailed explanation of the catalogue menu, refer to the documentation at [Shopware Catalogues](https://docs.shopware.com/en/shopware-6-en/catalogues).

### Orders: Managing Sales

The Orders section allows you to get an overview of incoming orders. This aspect will be explored in greater detail later in the course, providing a comprehensive understanding of order management.

### Customers: Your Key Focus

In the Customers section, you can view a comprehensive overview of your customers. This section also includes tools for managing PayPal disputes, with PayPal preinstalled as a payment method in your system.

### Content: Telling Your Story

The Content section is where you craft the shopping experiences for your customers. This includes defining general (static) shop pages, creating immersive landing pages, designing clear and focused listing pages, and detailing dedicated product pages. Additionally, this area allows you to upload and manage media used across your online shop.

### Themes: Reflecting Your Brand

In the Themes section, you configure the look and feel of your storefront. This customization helps in creating and reinforcing brand awareness, ensuring that the visual aspects of your store align with your brand identity.

### Marketing: Expanding Your Reach

The Marketing section is dedicated to administering newsletters and promotions for your products. This area helps you manage marketing efforts to enhance your store's visibility and attract more customers.

### Extensions: Tailoring Your Business

Finally, the Extensions section is where you manage both free and paid extensions, whether sourced from the store or custom-built. This functionality allows you to extend and tailor your installation to better suit your business requirements.

Understanding and effectively utilizing these building blocks will help you create a robust and successful online store tailored to your business needs.

### Settings: Set it up for you individually

The Settings section is crucial for tailoring your online store to meet your specific needs. This area encompasses a variety of configuration options, including shop settings, system settings, extension settings, and account settings. Shopware's extensive configurability allows you to adapt every aspect of your store to suit your unique business requirements, providing a high degree of flexibility.

<br /><br />
It's important to note that extensions you install may introduce additional navigation items within the Settings section. This means that as you customize your store with different extensions, you may encounter new settings and options to manage.

We will delve into these settings in detail in the upcoming units and courses, ensuring you gain a comprehensive understanding of how to configure your store effectively. For a complete and detailed description of all settings items, you can refer to the [Shopware documentation on configuration](https://docs.shopware.com/en/shopware-6-en/configuration). This resource will provide you with the necessary information to navigate and utilize the full range of settings available to you.

## Useful navigation and browser tips

Efficient navigation within your eCommerce platform can significantly enhance your productivity. Here are some useful tips for navigating through your modules and settings:

1. **Utilize Browser Functionalities**:
    - **Open Modules in New Tabs**: To streamline your workflow, take advantage of your browser’s ability to open links in new tabs or windows. This allows you to view multiple modules simultaneously. For instance, you might need to compare information between the Products and Orders sections. By using the "open in new tab" or "open in new window" options, you can easily switch between these views without losing your place.
    - **Use the “Go Back” Button**: Just like you would with other web applications, use the "go back" feature in your browser to return to previous pages within your eCommerce platform. This can be particularly useful if you navigate away from a page and need to return to your previous location quickly.
    - **Share URLs**: You can use the URL in your browser’s address bar to share specific pages or modules with colleagues. This can be helpful for collaborative tasks or for directing team members to particular sections of the platform.

By leveraging these browser functionalities, you can manage your eCommerce tasks more efficiently and ensure a smoother navigation experience.

## Useful settings

Let's cover some useful initial settings to do before continuing.

### Default Sales Channel

In this course, we will focus primarily on the Storefront sales channel. To streamline our workflow and ensure consistency, it’s important to set the Storefront as the default sales channel for all newly created products. Here’s how you can do that:

1. Begin by going to the **Settings** section of your eCommerce platform.
2. Within the **Shop** settings menu, locate and select **Products**.
3. At the top, you will see an option to choose the default sales channel. Select **Storefront** from this dropdown menu.

By setting the Storefront as your default sales channel, you ensure that all new products are automatically assigned to this channel, aligning with the focus of our course and simplifying the product management process.

## Suggested setup for this course

To effectively explore and learn about the functionalities in your eCommerce platform, it’s helpful to use multiple browser tabs. I recommend setting up two specific tabs:

1. **Shopware Administration**: Keep one tab dedicated to your Shopware Administration panel. This is where you will manage your store’s settings, products, and other backend functionalities.
2. **Storefront**: Open a second tab for your Storefront. To do this, click on the eye symbol located in the left menu. Ensure that this tab displays your default sales channel. This will allow you to view and interact with your online store from the customer’s perspective.

By utilizing these two tabs, you can seamlessly switch between the administration interface and the storefront, making it easier to understand how changes in the backend affect the customer experience. This approach will help you navigate and manage your eCommerce platform more effectively throughout the learning process.

<!--## Quick note on internationalization

Internationalization is a crucial aspect of expanding your eCommerce store’s reach and ensuring it meets the needs of a global audience. Here’s a brief overview of how internationalization works within your platform:

- **Importance of Internationalization**: In the long run, the ability to adapt your shop for different languages and regions is essential for growth and success. This process involves using snippets to translate and localize various elements of your store, including product descriptions, navigation menus, and more.
- **Coverage**: We will delve into the details of internationalization in a later section of the course. For now, rest assured that your platform is equipped to handle these needs effectively.

For more in-depth information, you can refer to the [Shopware internationalization documentation](https://docs.shopware.com/en/shopware-6-en/first-steps/internationalization?category=shopware-6-en/getting-started). This resource provides a comprehensive guide on how to implement and manage internationalization within your store.-->
