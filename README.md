# Food-Ordering-App-MERN-DEMO
<a href="https://drive.google.com/file/d/1RJzLnoh63AlDz6dUwKgoZcZq9fA9gZwX/view?usp=drive_link">Demo Video </a>

<hr>
# 🍔 OrderOnTheGo - Your On-Demand Food Ordering Solution

## 👥 Team Members
- Shaik Tayyibah  
- C Sunitha  
- V Anitha  
- V Sherylinpaul  

### 🧩 Roles in Project
- **C Sunitha & V Sherylinpaul**: Project Setup, Configuration, Frontend Development  
- **Shaik Tayyibah & V Anitha**: Backend Development, Database Development, Implementation & Execution  

---

## 📖 Project Overview

### 🎯 Purpose
**OrderOnTheGo** by SB Foods is a modern food ordering platform designed to simplify and enhance the online food ordering experience. It allows users to:

- Browse dishes with detailed information
- Place orders efficiently
- Receive real-time order confirmation
- Access a clean, user-friendly interface

Restaurants benefit by having a dashboard to manage menus, promotions, and incoming orders.

### 🚀 Key Features
- 🥘 Detailed dish info (price, reviews, promotions)
- 🌙 Late-night delivery support
- 💳 Simple checkout flow
- 🔔 Real-time order confirmation
- 🛠️ Admin dashboard for user/product/order management

---

## 🏗️ Architecture

### 🖼️ Frontend - React.js
- **Component-based architecture**
- **Routing** with `react-router-dom`
- **API calls** via `axios`

#### Key Functionalities:
- User registration/login
- Product listing
- Add to cart & manage cart
- Dynamic navigation and protected routes

### 🧠 Backend - Node.js + Express.js
- Express.js for RESTful APIs
- Middleware and route handling
- JWT-based authentication

### 💾 Database - MongoDB (via MongoDB Atlas)
- Mongoose for modeling application data

#### Schemas:
- **User**: username, email, password
- **Product**: name, category, price, etc.
- **Order**: userId, items, orderDate
- **Cart**: userId, productId, quantity
- **Admin**: categories, promotions
- **Restaurant**: name, menu items

---

## 🧰 Setup Instructions

### ⚙️ Prerequisites
- Node.js
- MongoDB Atlas account
- Express.js
- React.js
- Git
- Visual Studio Code

### 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   Install dependencies

Frontend:

bash
Copy
Edit
cd client
npm install

Backend:

bash
Copy
Edit
cd server
npm install
Start development servers

Frontend:

bash
Copy
Edit
npm start
Backend:

bash
Copy
Edit
npm start
Visit the App

arduino
Copy
Edit
http://localhost:3000


📁 Folder Structure
Frontend (/client)
bash
Copy
Edit
src/
├── components/          # Reusable components (Navbar, Login, etc.)
├── context/             # Context API (Auth, Cart)
├── images/              # Static assets
├── pages/
│   ├── admin/           # Admin dashboard pages
│   ├── customer/        # Customer-specific pages
│   └── restaurant/      # Restaurant dashboard pages
├── styles/              # CSS styling
├── Home.jsx             # Landing page
├── App.js               # Main app component
Backend (/server)
pgsql
Copy
Edit
server/
├── index.js             # Main entry point
├── Schema.js            # Mongoose schemas
├── package.json
├── package-lock.json
🔌 API Endpoints
🔐 Authentication
POST /api/auth/register
Registers a new user.

json
Copy
Edit
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "mypassword",
  "role": "customer"
}
POST /api/auth/login
Logs in a user and returns JWT.

json
Copy
Edit
{
  "email": "john@example.com",
  "password": "mypassword"
}
GET /api/auth/profile
Requires Bearer token (JWT).

json
Copy
Edit
{
  "id": "64d4fe9a01b12e...",
  "name": "John Doe",
  "email": "john@example.com",
  "role": "customer"
}
🥘 Products
GET /api/products
Returns all products.

POST /api/products
Adds a new product (Admin/Restaurant only).

📦 Orders
POST /api/orders
Places a new order.

json
Copy
Edit
{
  "userId": "123",
  "items": [ ... ],
  "total": 123
}
GET /api/orders/:userId
Returns all orders for a user.

🔐 Authentication Middleware
Protects routes like profile, cart, orders

Uses JWT to validate and authorize users

🖥️ User Interface
🖼️ Screenshots / Demo
📸 Click to view demo screenshots

🧪 Testing
🛠️ Strategy:
Manual testing using:

Postman for API testing

Browser for UI/UX testing

✅ Key Validations:
Form validations (login/register)

Order placement

Cart functionality

Authentication flow

To run tests:

bash
Copy
Edit
npm test
🐛 Known Issues
🔑 No password reset functionality

📧 No email verification

🔐 JWT stored in localStorage (XSS risk)

📦 No inventory/stock limit

💳 No payment gateway integration

🔮 Future Enhancements
🌐 Payment Gateway Integration (Stripe/Razorpay)

🔁 Real-Time Order Status Tracking using WebSockets or Firebase

📧 Email/OTP Verification

🔑 Password Reset Functionality

📱 Progressive Web App (PWA) support





















