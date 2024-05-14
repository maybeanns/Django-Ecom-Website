# E-Commerce Website-Comercio

## Overview
This project is a fully functional e-commerce website built using Django. It supports various features including user authentication, product management, shopping cart, order processing, and more. The platform is designed to be scalable, secure, and user-friendly.

## Table of Contents
1. [Features](#features)
2. [Tech Stack](#tech-stack)
3. [Installation](#installation)
4. [Configuration](#configuration)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

## Features
- **User Management**: Registration, login, logout, and profile management.
- **Product Management**: Adding, updating, and deleting products.
- **Shopping Cart**: Add to cart, view cart, update quantities, and remove items.
- **Order Processing**: Checkout, order history, and order tracking.
- **Admin Dashboard**: Manage products, orders, and users.
- **Search and Filtering**: Dynamic search and filters for products.
- **Reviews and Ratings**: User reviews and ratings for products.
- **Wishlist**: Add and manage wishlist items.
- **Payment Integration**: PayPal payment gateway, stripe

## Tech Stack
- **Backend**: Django, Django REST framework
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (development), PostgreSQL (production)
- **Deployment**: Docker, Gunicorn, Nginx

## Installation

### Prerequisites
- Python 3.x
- Django 3.x
- Docker (for deployment)

### Steps
1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/ecommerce-django.git
   cd ecommerce-django
   ```

2. **Create a virtual environment and activate it:**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

4. **Apply migrations:**
   ```sh
   python manage.py migrate
   ```

5. **Create a superuser:**
   ```sh
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```sh
   python manage.py runserver
   ```

## Configuration
- **Environment Variables**: Set environment variables in a `.env` file for sensitive information such as database credentials and secret keys.
- **Static and Media Files**: Configure paths for static and media files in `settings.py`.

### Example `.env` file
```sh
DEBUG=True
SECRET_KEY=your-secret-key
DB_NAME=your-database-name
DB_USER=your-database-user
DB_PASSWORD=your-database-password
DB_HOST=your-database-host
DB_PORT=your-database-port
```

## Usage

### Running the Server
- **Development**: `python manage.py runserver`
- **Production**: Use Docker and Gunicorn for deployment. See the [deployment guide](docs/deployment.md).

### Accessing the Admin Panel
- Navigate to `http://localhost:8000/admin/` and log in with the superuser credentials.

### Managing Products
- Use the admin panel to add, update, or delete products.

### User Operations
- Users can register, log in, view and edit their profiles, add products to their cart, proceed to checkout, and view their order history.

## Project Structure
```sh
ecommerce-django/
│
├── core/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── ...
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── ...
├── static/
│   ├── css/
│   ├── js/
│   └── ...
├── manage.py
├── requirements.txt
└── README.md
```

## Contributing
We welcome contributions! Please read our [contributing guidelines](CONTRIBUTING.md) for details on the process for submitting pull requests.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any queries or support, please contact:
- **Email**: m1annskhan@gmail.com
