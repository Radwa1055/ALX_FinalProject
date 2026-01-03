# E-commerce Product API (Second Chance Project)

## Project Overview
This project is an E-commerce Product API built with Django and Django REST Framework (DRF).  
It allows users to manage products and categories for an online marketplace.  
Users can create accounts, view products, and (if authenticated) create, update, or delete products.

---

## Features

### Product Management
- Create, Read, Update, Delete (CRUD) products
- Product attributes:
  - Name
  - Description
  - Price
  - Stock Quantity
  - Category
  - Image URL
  - Created Date
- Pagination for product listings
- Search products by name or category

### Category Management
- CRUD operations for categories
- Each product linked to a category

### Authentication & Permissions
- Only authenticated users can create, update, or delete products or categories
- Read-only access for unauthenticated users

### API Endpoints

#### Products
| Endpoint | Method | Description |
|----------|--------|-------------|
| /api/products/ | GET | List all products |
| /api/products/ | POST | Create a new product |
| /api/products/{id}/ | GET | Retrieve a single product |
| /api/products/{id}/ | PUT | Update a product |
| /api/products/{id}/ | DELETE | Delete a product |
| /api/products/?search={query} | GET | Search products by name or category |

#### Categories
| Endpoint | Method | Description |
|----------|--------|-------------|
| /api/categories/ | GET | List all categories |
| /api/categories/ | POST | Create a new category |
| /api/categories/{id}/ | GET | Retrieve a single category |
| /api/categories/{id}/ | PUT | Update a category |
| /api/categories/{id}/ | DELETE | Delete a category |

---

## Create virtual environment:
python3 -m venv venv
# venv\Scripts\activate   # Windows


# Install dependencies:
pip install -r requirements.txt


# Run the development server:
python manage.py runserver

# Access API at
Access API at


Project tested locally; PythonAnywhere deployment attempted but skipped for now.

Authentication handled via Django default user system.

Future improvements:

Token authentication (JWT)

Product reviews & ratings

Wishlist

Stock management

Discounts / Promotions





