# eCommerce Project

## Description

A fully functional eCommerce web application built with Laravel. This project provides a complete solution for online shopping with user and admin interfaces, including product listings, shopping carts, user registration, login, and admin functionalities such as managing products, categories, and orders.

## Features

-   **User Authentication**: Login and registration for users and admin.
-   **Product Management**: Add, edit, and delete products.
-   **Shopping Cart**: Add products to cart and proceed with checkout.
-   **Order Management**: Admin can view and manage orders.
-   **Responsive Design**: Optimized for mobile, tablet, and desktop devices.

## Prerequisites

Before you begin, ensure you have the following installed:

-   **PHP** (>=8.2 - 8.4)
-   **Composer**
-   **Node.js** (>=22.13.1)
-   **NPM** (>=10.9.2)
-   **MySQL** or **MariaDB** (for database)
-   **Git** (for version control)

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/JaydipDabhi/eCommerce.git
    ```

2. **Navigate to the project folder**:

```
cd eCommerce
```

3. **Install PHP dependencies**:
   This project uses Composer to manage PHP dependencies. To install them, run the following command:

-   ```
    composer update
    ```

4. **Install Node.js dependencies**:
   This project uses Node.js for front-end assets. To install the necessary dependencies, run:

-   ```
    npm install
    ```

5. **Copy .env.example to .env**:
   The .env file contains environment-specific variables (such as your database configuration). Copy the contents of .env.example to a new .env file:

-   ```
    cp .env.example .env
    ```

6. **Require Intervention Image 2.7 via Composer**:
   Run the following command in your terminal or command prompt:

-   ```
    composer require intervention/image:2.7
    ```

7. **Generate application key**:
   Laravel requires an application key for encryption and other security purposes. Generate the application key by running:

-   ```
    php artisan key:generate
    ```

8. **Run database migrations**:
   Laravel includes migrations to create the required database tables. Run the following command to set up the database schema:

-   ```
    php artisan migrate
    ```

9. **Installation for Shopping cart**:
   Install the package through Composer. Run the Composer require command from the Terminal:

-   ```
    composer require surfsidemedia/shoppingcart
    ```

10. **Configuration for Shopping cart**:
   To save cart into the database so you can retrieve it later, the package needs to know which database connection to use and what the name of the table is. By default the package will use the default database connection and use a table named shoppingcart. If you want to change these options, you'll have to publish the `config` file.

-   ```
    php artisan vendor:publish --provider="Surfsidemedia\Shoppingcart\ShoppingcartServiceProvider" --tag="config"
    ```

11. **Run the Laravel development server**:
   Start Laravel’s built-in development server by running:

-   ```
    php artisan serve
    ```

---

This is a complete installation guide for your eCommerce project to add in your GitHub `README.md` file. It includes all necessary steps to clone the project, install dependencies, set up the database, and run the application locally.
