# Scentopia – E-Commerce Platform for Fragrance Lovers

## Overview

**Scentopia** is a full-stack e-commerce platform dedicated to perfumes and fragrances.  
It provides a complete online shopping experience—from browsing products and managing carts to placing orders, making secure payments, and sharing reviews.

The platform is built with a **Node.js + Express backend** and **MongoDB** for data persistence, following a modular MVC-inspired architecture. It supports user authentication, product discovery, personalized recommendations, wishlists, reviews, order management, and payment processing.

Scentopia is designed to be **scalable, secure, and extensible**, making it suitable for real-world e-commerce use cases.

---


## Preview
<img width="1883" height="910" alt="image" src="https://github.com/user-attachments/assets/ace03708-c9e4-461a-b76a-b55ce8426e74" />https://scentopia.vercel.app/

---

## How It Works

### User Management & Authentication

- Users can register, log in, log out, and manage their profiles  
- Secure password handling using **bcrypt hashing**
- Supports:
  - Forgot password
  - Password reset
  - Email notifications via **Nodemailer**
- Admin-level user management:
  - View users
  - Update users
  - Delete users

---

### 2️Product & Category Management

- Products include:
  - Name
  - Price
  - Brand
  - Category
  - Stock count
  - Description
  - Image
- Categories support **hierarchical relationships** (parent/child)

**Product capabilities:**
- Create, update, delete products
- Text search with pagination
- Browse products by category

---

### 3️Shopping Cart & Wishlist

**Cart features:**
- Add products to cart
- Update product quantities
- View cart totals in real time

**Wishlist features:**
- Save favorite products
- Add or remove items
- Search and manage multiple wishlists

---

###  Reviews & Recommendations

- Customers can leave reviews with:
  - Title
  - Description
  - Rating
- Reviews are **validated and sanitized** to prevent malicious input
- Recommendations:
  - Tied to specific perfumes
  - Support curated or user-generated suggestions

---

###  Order Management

Orders store:
- User details
- Cart items
- Order status

**Admin capabilities:**
- View all orders
- Update order status
- Delete orders and restore product stock

---

### 6️Payment Processing

**Secure payment lifecycle:**
- Initiate payment
- Capture payment
- Refund payment
- Handle failures

**Supported features:**
- Transaction history
- Payment notifications
- Gateway integration (extensible for **CHAPA** or **Stripe**)

---

## Key Features

### User Features
- User registration & authentication
- Profile management
- Wishlist management
- Product reviews & ratings
- Secure checkout & order tracking

---

###  Product Features
- Product CRUD operations
- Category-based browsing
- Text search with pagination
- Stock management
- Product recommendations

---

### Cart & Order Features
- Add, update, and remove cart items
- Automatic total price calculation
- Order creation and management
- Inventory restoration on order deletion

---

### Payment Features
- Secure payment processing
- Payment capture & refunds
- Transaction history tracking
- Failure handling & notifications

---

###  Security & Validation
- Input validation with **express-validator**
- Data sanitization to prevent **XSS**
- Password hashing with **bcrypt**
- Environment-based configuration using **dotenv**

---

##  Architecture Highlights

- **Express.js** for RESTful APIs
- **MongoDB + Mongoose** for data modeling
- Modular controllers for:
  - Users
  - Products
  - Categories
  - Cart
  - Orders
  - Payments
  - Reviews
  - Wishlists
  - Recommendations
- Clean separation of concerns for maintainability

---

##  Future Enhancements
- Advanced recommendation engine
- Order analytics 
- Product image uploads with cloud storage
- Production-ready payment gateway integration


