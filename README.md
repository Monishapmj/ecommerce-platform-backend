
COMPANY : CODTECH IT SOLUTIONS 
NAME : MONISHA J 
INTERN ID : CT04DL69
DOMAIN : BACK END DEVELOPMENT 
DURATION : 4 WEEKS 
MENTOR : NEELA SANTHOSH KUMAR

# 🛒 E-Commerce Backend API

A robust, scalable, and secure backend system for an e-commerce platform. Built with Node.js, Express.js, and MongoDB, this API supports features like user authentication, role-based access, product and order management, and security best practices.

---

## 🚀 Features

### ✅ Core Functionalities
- **User Authentication** (JWT-based login & register)
- **Role-Based Access Control** (`admin`, `user`)
- **User Profile Management**
- **Product CRUD** (Admin only)
- **Order Creation & Management**
- **Cart Functionality**
- **Order Tracking**

### 🔐 Security & Best Practices
- JWT Authentication & bcrypt password hashing
- Rate limiting to prevent abuse
- Helmet for secure HTTP headers
- Input validation & sanitization
- CORS enabled for frontend-backend integration

---

## 🧱 Tech Stack

| Layer        | Tech                  |
|--------------|------------------------|
| Language     | JavaScript (ES6+)      |
| Runtime      | Node.js                |
| Framework    | Express.js             |
| Database     | MongoDB + Mongoose     |
| Auth         | JWT + bcrypt.js        |
| Validation   | express-validator      |
| Security     | Helmet, CORS, RateLimiter |
| Dev Tools    | Nodemon, Dotenv        |

---

## Prerequisites

- Node.js (v18.12.0 or higher)
- MongoDB (Running on the default port)
- npm (for dependency management)

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/AbdeIkader/eCommerce-Backend.git
cd eCommerce-Backend
npm install
```

Set up your environment variables in a `.env` file:

```env
MODE=dev
MONGO_URL=mongodb://127.0.0.1:27017/EcommerceC40
BASE_URL=http://localhost:3000/
```

## Running the Server

```bash
npm start
```

## API Endpoints

### Authentication
- POST `/signup`: Register a new user.
- POST `/signin`: Login for existing users.

### Address Management
- PATCH `/address`: Update an address for a user.
- DELETE `/address`: Remove an address for a user.
- GET `/address`: Retrieve all addresses for a user.

### Brand Management
- POST `/brand`: Add a new brand (admin).
- GET `/brand`: List all brands.
- PUT `/brand/:id`: Update a brand (admin).
- DELETE `/brand/:id`: Delete a brand (admin).

### Cart Management
- POST `/cart`: Add a product to the cart.
- GET `/cart`: Get the user's cart.
- POST `/cart/apply-coupon`: Apply a coupon to the cart.
- DELETE `/cart/:id`: Remove a product from the cart.
- PUT `/cart/:id`: Update product quantity in the cart.

### Category Management
- POST `/category`: Add a new category (admin).
- GET `/category`: List all categories.
- PUT `/category/:id`: Update a category (admin).
- DELETE `/category/:id`: Delete a category (admin).

### Coupon Management
- POST `/coupon`: Create a new coupon (admin/user).
- GET `/coupon`: List all coupons.
- PUT `/coupon/:id`: Update a coupon (admin/user).
- DELETE `/coupon/:id`: Delete a coupon (admin/user).
- GET `/coupon/:id`: Retrieve a specific coupon.

### Order Management
- POST `/order/:id`: Create a cash order (user).
- GET `/order`: Get a specific order (user).
- POST `/order/checkOut/:id`: Create a checkout session (user).
- GET `/order/all`: List all orders.

### Product Management
- POST `/product`: Add a new product (admin/user).
- GET `/product`: List all products.
- PUT `/product/:id`: Update a product (admin).
- DELETE `/product/:id`: Delete a product (admin).
- GET `/product/:id`: Retrieve a specific product.

### Review Management
- POST `/review`: Add a new review (user).
- GET `/review`: List all reviews.
- PUT `/review/:id`: Update a review (user).
- DELETE `/review/:id`: Delete a review (admin/user).

### Subcategory Management
- POST `/subcategory`: Add a new subcategory (admin/user).
- GET `/subcategory`: List all subcategories.
- PUT `/subcategory/:id`: Update a subcategory (admin/user).
- DELETE `/subcategory/:id`: Delete a subcategory (admin/user).

### User Management
- POST `/user`: Add a new user.
- GET `/user`: List all users.
- PUT `/user/:id`: Update a user.
- DELETE `/user/:id`: Delete a user.
- PATCH `/user/:id`: Change a user's password.

### Wishlist Management
- PATCH `/wishlist`: Add to wishlist (user).
- DELETE `/wishlist`: Remove from wishlist (user).
- GET `/wishlist`: Get all items in a user's wishlist.
  ## 📃 License
This project is open-source and free to use for educational and prototyping purposes.

## 🙋‍♀️ Author
Monisha J.
Designed and developed as part of backend internship at CodTech IT Solutions.


