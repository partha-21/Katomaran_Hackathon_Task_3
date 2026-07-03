# Project Description

## Overview

This project is a web automation testing framework developed using Java, Playwright, Maven, and JUnit 5. The framework is designed to automate login functionality testing for the Tichi application while following industry-standard automation practices. It provides a clean, modular, and scalable structure that can be easily extended for future test scenarios.

## Framework Design

The project follows the Page Object Model (POM) design pattern to improve maintainability, readability, and code reusability. Application pages and their corresponding actions are separated from test logic, making the framework easier to maintain and reducing duplication.

## Key Components

### Browser Management

The `BrowserFactory` class is responsible for browser initialization and management. It creates Playwright instances and applies execution settings such as browser mode and runtime configurations.

### Configuration Management

The framework uses an external `config.properties` file along with a `ConfigReader` utility class to manage configurable values. This allows changes to execution settings without modifying source code.

### Page Layer

The `LoginPage` class contains all login page elements and user interactions, including:

* Email input handling
* Password input handling
* Login submission
* Validation for successful and unsuccessful login scenarios

### Test Layer

JUnit 5 is used as the test framework for implementation of test cases.

Implemented test scenarios include:

1. Valid Login Test

   * Verifies successful authentication
   * Validates the expected welcome message after login

2. Invalid Login Test

   * Verifies behavior for incorrect credentials
   * Ensures users remain on the login page when authentication fails

## Technologies Used

* Java
* Playwright
* Maven
* JUnit 5

## Conclusion

This framework demonstrates best practices in automation framework development through modular architecture, configuration-driven execution, and maintainable test implementation. It provides a solid foundation for future enhancements such as reporting integration, CI/CD implementation, and cross-browser testing support.
