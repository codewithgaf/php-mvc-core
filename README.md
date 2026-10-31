# PHP MVC Core

### A Lightweight PHP MVC Framework Built from Scratch

A lightweight PHP MVC framework core designed to provide a structured foundation for building web applications using PHP and Object-Oriented Programming (OOP).

This project explores the fundamentals of MVC architecture by implementing essential framework components, including routing, controllers, models, views, request and response handling, session management, middleware support, and database integration.

The goal is to understand how PHP frameworks organize application logic and manage the request-response lifecycle.

---

## Overview

**PHP MVC Core** is a personal backend development project focused on understanding and implementing the core concepts behind modern PHP frameworks.

Instead of relying entirely on an existing framework, this project builds essential components from scratch to explore how different parts of a web application communicate and work together.

It follows the Model-View-Controller (MVC) architectural pattern to encourage separation of concerns, maintainability, and organized application development.

## Features

The current implementation includes:

- **MVC Architecture** – Separates application logic into Models, Views, and Controllers.
- **Routing System** – Handles incoming requests and resolves application routes.
- **Controller Management** – Provides a base controller for rendering views and registering middleware.
- **Model Abstraction** – Provides a base model with data loading and validation capabilities.
- **Form Validation** – Supports required, email, minimum length, maximum length, matching, and unique validation rules.
- **View Rendering** – Provides a view component for rendering application views.
- **Request Handling** – Provides request-related functionality.
- **Response Handling** – Provides response management functionality.
- **Session Management** – Handles session-related operations.
- **Database Integration** – Includes a database component for application database access.
- **Middleware Support** – Provides middleware registration and management through controllers.
- **User Authentication Foundation** – Includes login, logout, and authenticated-user handling in the application core.
- **Event Hooks** – Provides before-request and after-request event constants and event listener registration.

*Note: These features describe the current implementation. Some components may require additional configuration or integration within a host application.*

## Architecture

The framework follows the Model-View-Controller (MVC) design pattern.

```text
        Client Request
              |
              v
         Application
              |
              v
            Router
              |
              v
          Controller
           /      \
          /        \
         v          v
       Model       View
         |           |
         v           |
      Database       |
         |           |
         v           v
       Data      HTML Output
          \         /
           \       /
             Response
                 |
                 v
              Client
```

### Core Components

| Component | Responsibility |
|---|---|
| Application | Initializes and coordinates framework components. |
| Router | Resolves incoming requests to application routes. |
| Controller | Handles application actions and view rendering. |
| Model | Manages application data and validation rules. |
| View | Handles view rendering. |
| Request | Provides request handling functionality. |
| Response | Provides response management functionality. |
| Session | Manages session operations. |
| Database | Provides database integration. |
| Middleware | Provides a foundation for middleware registration. |

## Project Structure

```text
php-mvc-core/
│
├── Form/
│
├── db/
│
├── exception/
│
├── middlewares/
│
├── Application.php
├── Controller.php
├── Model.php
├── Request.php
├── Response.php
├── Router.php
├── Session.php
├── UserModel.php
├── View.php
│
├── composer.json
└── README.md
```

## Technologies Used

- PHP
- Object-Oriented Programming (OOP)
- Model-View-Controller (MVC)
- Composer
- PSR-4 Autoloading
- SQL / Database Integration

## Getting Started

### Prerequisites

Before using this project, make sure you have:

- PHP installed.
- Composer installed.
- A web server or PHP development environment.
- A database server if using database-related components.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/codewithgaf/php-mvc-core.git
```

**2. Navigate to the project directory**

```bash
cd php-mvc-core
```

**3. Generate the Composer autoloader**

```bash
composer dump-autoload
```

The project uses Composer PSR-4 autoloading with the namespace prefix:

```php
gaf\phpmvc\
```

mapped to the project root directory.

### Integration

This repository contains framework core components rather than a complete standalone application.

To use it within a PHP application:

1. Include the Composer autoloader.
2. Configure the application root directory.
3. Prepare the required application configuration.
4. Initialize the Application class.
5. Register application routes and controllers.
6. Configure database settings if database functionality is required.
7. Connect the framework to your application's entry point.

Refer to the source code for the current implementation and required configuration.

## Learning Objectives

This project provides practical experience with:

- Understanding MVC architecture.
- Implementing object-oriented PHP.
- Building a custom routing mechanism.
- Organizing application components.
- Understanding request and response handling.
- Implementing reusable model validation.
- Working with Composer and PSR-4 autoloading.
- Exploring database integration.
- Understanding session-based authentication.
- Exploring middleware and application event hooks.

## Future Improvements

The framework is a work in progress. Potential improvements include:

- Enhanced routing and HTTP method handling.
- Improved exception handling.
- Expanded middleware execution pipeline.
- More comprehensive form validation.
- Improved database abstraction.
- Stronger authentication and authorization mechanisms.
- CSRF protection and additional security features.
- Automated unit and integration tests.
- Better documentation and usage examples.
- Improved configuration management.

## Project Status

**Status: Work in Progress**

This project is continuously evolving as I strengthen my PHP development skills and explore backend software engineering concepts.

Some components may require further development, testing, and security improvements before being suitable for production use.

## Author

**Gafour Panolong**

Aspiring Software Engineer | Backend Development | DevOps Engineering

- GitHub: [@codewithgaf](https://github.com/codewithgaf)
- LinkedIn: [Gafour Panolong](https://www.linkedin.com/in/gafourpanolong/)

---

### Built with PHP and a passion for understanding how things work under the hood.

*Learn continuously. Build meaningfully. Solve real problems.*
