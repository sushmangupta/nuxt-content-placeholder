---
title: "Kickstart Shopware 6"
slug: "kickstart-shopware"
description: "How to get going with your individual instance of Shopware"
icon: "" # svg, png? dark mode?
authors: [d.hoeting]
visibility: "public"
---
# Kickstart Shopware 6
When embarking on your journey with Shopware, there are several paths you can take to get started, each offering distinct advantages depending on your needs and preferences. As you may recall from before, Shopware offers two primary deployment options: self-hosted and cloud.

The cloud option is known for being the most opinionated, offering a straightforward and hassle-free experience. The cloud solution is particularly appealing due to its ease of use and the minimal technical expertise required to get started.

In contrast, the self-hosted deployment provides a higher degree of freedom and flexibility. This option allows you to have more control over your Shopware environment, including customization and configuration. However, this increased flexibility comes at the cost of requiring a more significant technical skill set and resources to host and manage the system effectively.

To help you navigate these options and determine the best fit for your situation, it is essential to explore the various alternatives for getting started with Shopware. Each approach has its unique benefits and considerations, and understanding these will enable you to make an informed decision tailored to your specific requirements.

## Quick and easy - Shopware Sandbox

To begin exploring Shopware efficiently and without the complications of local software installation, you can opt for the **Shopware Sandbox**, which provides a swift and straightforward entry point. This method offers the benefit of bypassing the need for local server setup while still granting you the flexibility to transition to other distribution models later on.

The Shopware Sandbox is designed specifically for developers who wish to experiment with app and storefront development in a controlled environment. It is important to note that the sandbox is intended solely for development purposes and will be automatically deleted after one month. It is not meant to function as a live shop at any time. Despite this, the sandbox remains an accessible and practical option for getting started with Shopware immediately.

To set up your Shopware Sandbox, follow these steps:

1. **Create a Shopware account and log in**: Begin by visiting [account.shopware.com](https://account.shopware.com/) and register a new account if you don't happen to already have one - in that case, just log in. <!-- Screenshot -->
2. **Create a Developer Sandbox**: Proceed to create a developer sandbox - this is presented to you right on the Dashboard in the Shopware Account. The setup process might take a few minutes, during which your instance will be prepared for use. <!-- Screenshot -->
3. **Access your Sandbox**: After the sandbox has been created, log into the Shopware administration panel using your existing account credentials. At this point, you will have access to explore and work with Shopware. <!-- Screenshot -->

With the sandbox in place, you can continue progressing through the course using this environment. Note that this option is actually **intended for developers** - and you will notice that by what is highlighted on the Dashboard - hence you cannot go live in this environment and the Shopware Store is disabled. Still, you can explore the functionality of Shopware. The developer sandbox reflects the **Evolve** plan!

## Installing yourself - Shopware onPremise

When considering the deployment of Shopware, the two primary options—cloud and on-premise—each come with their own set of advantages and disadvantages.

**Advantages of Self-Hosted Deployment**

One of the significant advantages of opting for an self-hosted deployment is the **full control and flexibility** it offers. With self-hosted Shopware, you have the ability to tailor every aspect of your environment to meet your specific needs. This includes customizing the system configurations, integrating with other tools and applications, and making adjustments that align perfectly with your business processes.

Additionally, the self-hosted solution is truly **owned by you**. As default, this reflects a Community Edition. However, you can choose to book a plan and benefit from additional features and services.

**Challenges of Self-Hosted Deployment**

However, this flexibility does not come without its challenges. **Complexity** is a notable challenge, as managing an self-hosted deployment involves navigating various technical aspects and configurations. This increased complexity can lead to a steeper learning curve and potential difficulties in maintaining the system.

Furthermore, self-hosted setups require additional effort for **hosting**. You must handle the server management, ensure adequate security measures, and perform regular maintenance tasks. This adds an extra layer of responsibility compared to cloud solutions where much of the infrastructure is managed for you.

Additionally, **technical know-how** is essential for a successful self-hosted deployment. Without a solid understanding of the technical requirements and management practices, you might encounter challenges in setting up and maintaining your system effectively.

Overall, while self-hosted deployment offers significant control and flexibility, it also demands a higher level of technical expertise and involves more complex management and hosting responsibilities.

### Installation of Shopware in an On-Premise Environment

Installing Shopware in an on-premise environment requires a certain level of technical expertise. This process involves several critical steps and considerations to ensure a successful setup.

#### Access to a Web Server

To install Shopware, you must have access to a web server. This can be done on your local machine; however, if you choose this route, the installation will be accessible only to you or those on your local network. For broader access, it is advisable to install Shopware on a web server that is accessible over the internet.

#### System Requirements

Before beginning the installation, it is crucial to thoroughly check the system requirements to ensure your environment meets all necessary criteria. Comprehensive documentation on these requirements can be found at the following links:

- [Shopware System Requirements](https://docs.shopware.com/en/shopware-6-en/first-steps/system-requirements?category=shopware-6-en/getting-started)
- [Shopware Developer Documentation on Requirements](https://developer.shopware.com/docs/guides/installation/requirements.html)

#### Installation Process

The installation process for Shopware can be guided by detailed documentation available online. To install Shopware yourself, follow the instructions outlined here: [Shopware Installation Guide](https://docs.shopware.com/en/shopware-6-en/first-steps/installing-shopware-6?category=shopware-6-en/getting-started).

In a nutshell:

1. **Download the Installer**: Obtain the installer from the official Shopware download page: [Shopware Download](https://www.shopware.com/en/download/).
2. **Prepare the Installation**: Create a folder on your web server and place the `shopware-installer.phar.php` file into it.
3. **Run the Installer**: Access the installer through your web browser. This will initiate the installer and guide you through the initial setup wizard, which will help you complete your Shopware installation.
4. **Follow the Steps**: Proceed with the installation by following the on-screen instructions. <!-- Screenshot -->

If you encounter any issues, refer to the comprehensive installation guide for troubleshooting: [Shopware Installation Guide](https://docs.shopware.com/en/shopware-6-en/first-steps/installing-shopware-6?category=shopware-6-en/getting-started).

### Alternatives to the Installer

There are alternative methods to running Shopware locally or on your server, which may offer different features or ease of use:

1. **Symfony Flex**: This method leverages Symfony Flex for installation. For more details, visit the [Symfony Flex Guide](https://developer.shopware.com/docs/guides/installation/template.html).
2. **Devenv**: Another option is using Devenv, which provides a pre-configured development environment for Shopware. More information is available in the [Devenv Documentation](https://developer.shopware.com/docs/guides/installation/devenv.html).

These alternatives may offer additional features or simplified installation processes, depending on your specific needs and technical proficiency.

<!-- shorten what was covered already -->
<!-- more direction to other resources -->
