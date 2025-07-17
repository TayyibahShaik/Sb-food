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

Step 2: Install All Dependencies
Run the following commands in the root of your project directory:
# Install backend dependencies
cd server
npm install

.

📁 Folder Structure
Frontend (/client)
<br>
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
<br>
Backend (/server)
<br>
server/
├── index.js             # Main entry point
├── Schema.js            # Mongoose schemas
├── package.json
├── package-lock.json


# Install frontend dependencies
cd ../client
npm install
<br>
📂 Backend Dependencies (/server)
The following packages will be installed for the backend:
| Package       | Purpose                                |
| ------------- | -------------------------------------- |
| express       | Web framework for building the API     |
| mongoose      | MongoDB object modeling tool           |
| dotenv        | Load environment variables             |
| cors          | Enable Cross-Origin Resource Sharing   |
| bcryptjs      | Password hashing                       |
| jsonwebtoken  | JWT-based authentication               |
| nodemon (dev) | Auto-reloads server during development |
<br>
<br>
📂 Frontend Dependencies (/client)
The following packages will be installed for the frontend:<br>

| Package          | Purpose                                |
| ---------------- | -------------------------------------- |
| react            | Frontend library for building UI       |
| react-router-dom | Client-side routing                    |
| axios            | HTTP requests to backend APIs          |
| react-icons      | Icons for UI components                |
| dotenv           | Load client-side environment variables |
<br>
Step 3: Start the Application<br>
Use the following commands in two separate terminals:
cd server
npm start
<br>
🔌 API Endpoints
🔐 Authentication
POST /api/auth/register
Registers a new user.<br>
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "mypassword",
  "role": "customer"
}
.<br>
🔐 Authentication Middleware
Protects routes like /profile, /orders, /cart

Validates JWT from headers

Redirects unauthenticated users
<br>
🖥️ User Interface
🖼️ Screenshots / Demo

<img width="1023" height="542" alt="image" src="https://github.com/user-attachments/assets/21a075ca-a073-4fcb-a3cb-1d040ed2cee7" /><br>

**🧪 Testing<br>**
🛠️ Strategy
Manual testing using:
Postman (for API requests)
Browser (for UI interactions)

<b>✅ Validated Flows</b>
User registration and login
Product listing and cart
Order placement
Dashboard access for admin and restaurant

<b>To run tests:<</b><br>
npm test
<br>

<br>
<b>🐛 Known Issues</b><br>

🔑 No password reset functionality
📧 No email verification
🔐 JWT stored in localStorage (XSS risk)
📦 No inventory/stock limit
💳 No payment gateway integration

**🔮 Future Enhancements**<br>

🌐 Payment Gateway Integration (Stripe, Razorpay)
🔁 Real-Time Order Tracking (WebSockets/Firebase)
📧 Email/OTP Verification for Sign-Up
🔑 Forgot Password & Secure Reset Flow
📱 PWA (Progressive Web App) Capabilities





























