---
title: "Best practices for maintaining code quality"
slug: "maintaining-code-quality"
description: "Learning unit about basic plugin structure"
icon: ""
authors: ["Micha Hobert"]
visibility: "public"
---

# Learning Objectives

By the end of this unit, you will be able to:

- Write an e2e test for a Shopware app
- Know how to run tests in Shopware

# Introduction
Maintaining code quality is essential for the long-term success of your project. It ensures that your code is readable, maintainable, and scalable. In this learning unit, you will learn about best practices for maintaining code quality in Shopware.

## Version control
Code quality begins at your base. This sounds kind of silly in 2024, but it is highly recommended to use GIT for your extension, app or bundle.

## Automated testing
As mentioned in the last learning unit, automated testing is a crucial part of maintaining code quality. It helps you catch bugs early in the development process and ensures that your code works as expected. There are different types of automated testing, such as unit tests, integration tests, and end-to-end tests.

## Code reviews
Code reviews are another essential part of maintaining code quality. They help you catch bugs, improve code quality, and ensure that your code follows best practices. Code reviews should be done by your peers or a senior developer who can provide valuable feedback.

It should always seen as a learning opportunity and not as a critique of your work. It is a great way to learn from others and improve your coding skills.

## Code quality tools
There are many tools available that can help you maintain code quality. Some popular tools include:

- PHPStan
- ESLint
- Stylelint
- SonarQube

These tools can help you catch bugs, enforce coding standards, and improve code quality.

## Documentation
Documentation is another essential part of maintaining code quality. It helps you and other developers understand your code, its purpose, and how to use it. Good documentation can save you time and prevent misunderstandings.

It also helps new developers to get started with your codebase and understand the architecture of your project.

## Continuous integration
Continuous integration is a development practice that helps you catch bugs early in the development process. It involves automatically building, testing, and deploying your code whenever a change is made. This ensures that your code is always in a working state and helps you catch bugs before they reach production.

## Code quality guidelines
Code quality guidelines are a set of rules and best practices that help you maintain code quality. They cover things like coding standards, naming conventions, and code structure. Following code quality guidelines can help you write better code and improve the overall quality of your project.

## Refactor code regularly
Refactoring is the process of improving your code without changing its behavior. It helps you keep your code clean, maintainable, and scalable. Regularly refactoring your code can help you catch bugs, improve code quality, and ensure that your code is easy to maintain.

It helps to set a quarterly event in your company or workspace to refactor code. This way you can ensure that your codebase is always up to date and follows the latest best practices. If you are publishing your extension or app in the store this often comes naturally, as you need to update your code to the latest Shopware version.

Talking about the store, there are also guidelines for extensions that are published in the store.

You can find a extended version of the [quality guidelines](https://developer.shopware.com/docs/resources/guidelines/testing/store/quality-guidelines-plugins/) in the official Shopware documentation.


# Quiz

1. What version control system is recommended for maintaining code quality?
   [ ] SVN
   [x] GIT
   [ ] Mercurial
   [ ] CVS
2. What is the purpose of code reviews?
   [ ] To critique your work
   [x] To catch bugs and improve code quality
   [ ] To slow down the development process
3. What is the purpose of code quality tools?
   [x] To catch bugs, enforce coding standards, and improve code quality
   [ ] To slow down the development process
   [ ] To make your code less readable