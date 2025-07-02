# PyShop: A Simple Django E-commerce Project

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Django](https://img.shields.io/badge/Django-5.x-092E20?style=for-the-badge&logo=django)
![Database](https://img.shields.io/badge/Database-SQLite-07405E?style=for-the-badge&logo=sqlite)
![Frontend](https://img.shields.io/badge/Frontend-HTML%2FCSS%2FBootstrap-orange.svg)

## Project Overview

PyShop is a foundational e-commerce web application built with Django, designed to demonstrate core web development concepts, including database management, user interface rendering, and admin functionality. This project serves as a practical learning experience in creating a basic online shop where products can be listed, viewed, and managed.

## Problem Solved

This project addresses the fundamental requirement of displaying products online. It provides a simple, yet effective, platform for:
-   Showcasing a catalog of products.
-   Providing detailed information for each product.
-   Allowing administrative control over product inventory.

## Features

-   **Product Catalog:** Browse a list of available products.
-   **Product Details:** View individual product pages with descriptions, prices, and images.
-   **Admin Panel:** Utilize Django's powerful built-in admin interface to easily add, update, and delete products.
-   **Basic UI:** Simple and clean user interface for navigation.

## Technologies Used

* **Backend:**
    * [Python](https://www.python.org/) - The core programming language.
    * [Django](https://www.djangoproject.com/) - High-level Python web framework for rapid development.
    * [SQLite](https://www.sqlite.org/index.html) - Default database for development, lightweight and file-based.
* **Frontend:**
    * HTML5, CSS3 - For structuring and styling web pages.
    * [Bootstrap](https://getbootstrap.com/) - Front-end framework for responsive and modern design.

## Installation & Setup

Follow these steps to get PyShop up and running on your local machine.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/meez-111/pyshop-django-shop.git](https://github.com/meez-111/pyshop-django-shop.git)
    cd pyshop-django-shop
    ```

2.  **Create and activate a virtual environment:**
    It's highly recommended to use a virtual environment to manage project dependencies.
    ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate
    ```

3.  **Install dependencies:**
    * Make sure you have your `requirements.txt` file in the project root.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Apply database migrations:**
    ```bash
    python manage.py makemigrations products
    python manage.py migrate
    ```

5.  **Create a superuser (for admin access):**
    You'll need an admin account to manage products through the Django admin panel.
    ```bash
    python manage.py createsuperuser
    ```
    Follow the prompts to create a username, email, and password.

6.  **Run the development server:**
    ```bash
    python manage.py runserver
    ```
    The application will be accessible at `http://127.0.0.1:8000/`.

## Usage

1.  **Browse Products:**
    * Open your web browser and go to `http://127.0.0.1:8000/products`.

2.  **Manage Products via Admin Panel:**
    * Go to `http://127.0.0.1:8000/admin`.
    * Log in using the superuser credentials you created.
    * From the admin dashboard, you can add new products, edit existing ones, and manage categories. Remember to upload images for your products to `media/products/`.

## Important Notes & Best Practices

* **`.gitignore`:** Ensure your `.gitignore` file correctly excludes sensitive data and unnecessary files like `db.sqlite3` (your local development database) and the `media/` folder (for user-uploaded files). These should never be committed to version control, especially in public repositories. If these were committed previously, use `git rm --cached` to stop tracking them.
* **`requirements.txt`:** Always maintain an up-to-date `requirements.txt` file (by running `pip freeze > requirements.txt` after installing dependencies) to ensure anyone can easily install all necessary libraries for your project.
* **`SECRET_KEY`:** For production environments, your Django `SECRET_KEY` should be stored securely as an environment variable, not directly in `settings.py`.
* **Static & Media Files:** In a production deployment, static and media files are served differently (e.g., via a web server like Nginx or a cloud storage solution).

## Future Enhancements (Ideas for expanding the project)

-   **Shopping Cart & Checkout:** Implement functionality for users to add items to a cart, proceed to checkout, and place orders.
-   **User Authentication:** Allow users to register, log in, and manage their profiles.
-   **Search Functionality:** Add a search bar to filter products by name or description.
-   **Payment Gateway Integration:** Integrate with a mock or real payment gateway (e.g., Stripe, PayPal).
-   **Product Reviews:** Enable users to leave reviews for products.
-   **Deployment:** Deploy the application to a cloud platform (e.g., Heroku, Render, AWS, DigitalOcean) to make it publicly accessible.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Any contributions are welcome!

## Contacts

**LinkeIn:** [My LinkedIn](https://www.linkedin.com/in/moaz-sabra-3a7565330/)

**Email:** [My Email](meez.sabra.111@gmail.com)