---
title: "Introduction to testing in Shopware"
slug: "intro-testing-shopware"
description: "How to run tests in Shopware"
icon: ""
authors: ["Micha Hobert"]
visibility: "public"
---


# Learning Objectives

By the end of this unit, you will be able to:

- Write an e2e test for a Shopware app
- Know how to run tests in Shopware

# Introduction

In this learning unit, we will take a closer look at the testing possibilities in Shopware. Testing is an essential part of software development. It helps you to ensure that your code works as expected and that you don't introduce any bugs.

## Real-world example

Your plugin/app is done, and you want to make sure that it works as expected. You can write tests to check if the functionality is working correctly. This way, you can be sure that your plugin/app works as expected even after future changes.


## Convince your boss

Testing is an essential part of software development. It helps you to ensure that your code works as expected and that you don't introduce any bugs. By writing tests, you can be sure that your code works as expected even after future changes. This will save you time and money in the long run.

Often this is seen as a last step in the development process, but it is essential to write tests from the beginning. This way, you can ensure that your code works as expected and that you don't introduce any bugs.

If testing is not part of your development process yet, you should convince your boss to include it and prepare a pitch with numbers and facts. In the long run, it will save you and the company a lot of time and money.



## Unit tests

Unit tests are used to test individual units of code, like functions or classes. They are isolated from the rest of the codebase and should be fast to execute.

### PHPUnit

Shopware uses PHPUnit for unit tests. If you have used the plugin:create command to create your plugin, the necessary PHPUnit configuration is already set up for you.

You will find all necessary information about integration tests, mocking services in the [official documentation](https://developer.shopware.com/docs/guides/plugins/plugins/testing/php-unit.html) 

### Jest

Writing unit tests in Jest for the storefront and administration is also possible. You can find more information in the [official documentation](https://developer.shopware.com/docs/guides/plugins/plugins/testing/jest.html)

## End-to-end tests

End-to-end tests are used to test the whole application or a specific feature. They simulate a real user interaction with the application. For example checking if your newly added button on the product detail page is really there and has the correct color.

### Cypress

Shopware uses [Cypress](https://www.cypress.io/) for end-to-end tests. There is an [e2e-testsuite](https://github.com/shopware/e2e-testsuite-platform) available in the Shopware repository. It will kickstart your testing journey with Shopware. 

The [official developer documentation](https://developer.shopware.com/docs/guides/plugins/plugins/testing/end-to-end-testing.html) gives you a great overview of how to install the testsuite and run the first tests.


## Quiz

1. How can your convince your boss to include testing in the development process?
  [x] Prepare a pitch with numbers and facts
  [] Tell him that you will quit if he doesn't include testing
  [] Tell him that testing is not necessary
2. What is the purpose of unit tests?
  [] Test the whole application
  [x] Test individual units of code
  [] Test the user interaction
3. What should be used for end-to-end tests in Shopware?
  [] Jest
  [] PHPUnit
  [x] Cypress