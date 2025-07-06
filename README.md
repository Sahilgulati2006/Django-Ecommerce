# 🛍️ Django eCommerce Website

A fully functional eCommerce web application built with **Django**, integrated with **PayPal for payments**, and designed to support both guest and registered users. This project implements cart management, checkout, dynamic order summaries, and shipping functionality with a clean Bootstrap UI.

---

## 🚀 Features

- 🛒 Add/Remove items to cart
- 👤 Guest and authenticated user checkout
- 📦 Shipping information management
- 💳 Integrated PayPal payment system
- 📊 Dynamic order summary & cart total calculation
- 📦 Admin can track order items and shipping info
- 📸 Product image support
- 📁 Cookie-based cart management for anonymous users
- 🔒 CSRF protection and secure transaction handling

---
## 📁 Project Structure

```
ecommerce/
├── config/                # Django project settings
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── static/                # Static files
│   ├── css/
│   │   └── main.css
│   ├── images/
│   └── js/
│       └── cart.js
│
├── store/                 # Store app
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── utils.py
│   ├── views.py
│   ├── migrations/
│   └── templates/
│       └── store/
│           ├── main.html
│           ├──

```

## 🧰 Tech Stack

- **Backend:** Django 3.x+
- **Frontend:** HTML, Bootstrap, JavaScript
- **Payments:** PayPal JavaScript SDK
- **Database:** SQLite (default, but easily swappable to PostgreSQL)
- **Static Files Handling:** Django staticfiles

---

## 🧑‍💻 Getting Started

### 📦 Prerequisites

- Python 3.8+
- pip
- Virtualenv (recommended)

### 🔧 Setup

```bash
git clone https://github.com/yourusername/django-ecommerce.git
cd django-ecommerce

# Create and activate virtual environment
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

# Run server
python manage.py runserver
```

Open your browser and go to: `http://127.0.0.1:8000/`

---

## 💳 PayPal Setup

To use PayPal payments:

1. Go to [PayPal Developer Console](https://developer.paypal.com)
2. Create a sandbox business account.
3. Get the **Client ID** from your sandbox app.
4. Replace the `client-id` in your HTML file:

```html
<script src="https://www.paypal.com/sdk/js?client-id=YOUR_CLIENT_ID&currency=USD"></script>
```

---

## 🗃️ Models Overview

- **Customer:** One-to-one with Django User model
- **Product:** Represents the products in the store
- **Order:** Links customer and products, tracks cart state
- **OrderItem:** Tracks product and quantity in each order
- **ShippingAddress:** Stores shipping information

---

## 📸 Screenshots

> Replace the placeholders below with actual image links.

| Store Page | Cart Page | Checkout Page |
|------------|-----------|----------------|
| ![](path-to-store.png) | ![](path-to-cart.png) | ![](path-to-checkout.png) |

---


## 🙋‍♂️ Author

**Sahil Gulati**  
[GitHub](https://github.com/Sahilgulati2006) • [LinkedIn](https://www.linkedin.com/in/sahil-gulati-b991a62a2/)

---
