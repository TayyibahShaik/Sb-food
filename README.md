# Food-Ordering-App-MERN-DEMO
<a href="https://drive.google.com/file/d/1RJzLnoh63AlDz6dUwKgoZcZq9fA9gZwX/view?usp=drive_link">Demo Video </a>

<hr>
<b>🍕Food-Ordering-App-MERN-DEMO<b/></b>
1.	Introduction<br>
•	Project Title: OrderOnTheGo: Your On-Demand Food Ordering Solution <br>
•	Team Members: Shaik Tayyibah, C Sunitha, V Anitha, V Sherylinpaul.<br>
2.	Project Overview<br>
•	Purpose: The SB Foods project, also known as OrderOnTheGo, is developed to enhance the way people order food online by offering a seamless, efficient, and user-friendly web platform. It aims to provide users with a smooth and enjoyable food ordering experience by allowing them to easily explore various dishes, view detailed information, and place orders with minimal steps. 
	By focusing on simplicity and personalization, SB Foods ensures that users can find meals that match their tastes and preferences quickly. In addition to serving customers, the project also supports restaurants by giving them a platform to present their offerings and manage orders efficiently. Overall, the project’s goal is to simplify online food ordering, improve customer satisfaction, and bridge the gap between food lovers and restaurants in a modern, digital environment.<br>
•	Features: OrderOnTheGo by SB Foods is a modern food ordering platform designed to make online food ordering easy, fast, and convenient. It offers detailed dish information, instant order confirmation, and a user-friendly interface. <br>
	A real-life scenario shows how the app helps users like Lisa, a student needing a quick meal at midnight, to order food in minutes and continue her work undisturbed.<br>
1.	Easy dish selection with full details (reviews, price, promotions)
2.	Late-night delivery support
3.	Simple checkout process (name, address, payment)
4.	Real-time order confirmation
5.	Admin dashboard for managing users, products, and orders

3.	Architecture
•	Frontend: The frontend of the application is developed using React.js, which enables a component-based, modular, and scalable architecture. The structure is organized into the following key areas: 
a)	 App Setup: A React app is created in the client folder with necessary libraries like react-router-dom and axios. Routing is set up to manage different pages
b)	UI Design: Reusable components are created for layout, navigation, and styling. Pages are designed for user interaction and easy navigation.
c)	 Key Functionalities:
	Register & Login: Users can register and log in securely using forms and API integration.
	All Products Page: Displays a list of available food items fetched from the backend.
	Add to Cart: Users can add products to their cart. The cart is managed using React state or context and updates in real time.

•	Backend:  Create a new directory for your project and set up a package.json file using the npm init command. Install necessary dependencies such as Express.js, Mongoose, and other required packages.

a)	 Node.js and npm: Install Node.js, which includes npm (Node Package Manager), on your development machine. Node.js is required to run JavaScript on the server side. • Download: https://nodejs.org/en/download/

b)	 Express.js: Express.js is a web application framework for Node.js. Install Express.js to handle server-side routing, middleware, and API development. 

•	Database: Create database in cloud
1.	Install Mongoose.
2.	Create database connection.

	Reference Article: https://www.mongodb.com/docs/atlas/tutorial/connect-to-your-cluster/

a)	User Schema: <br>
• Schema: user Schema 
• Model: ‘User’ 
• The User schema represents the user data and includes fields such as username, email, and password. 

b)	Product Schema: <br>
• Schema: product Schema 
• Model: ‘Product’ 
• The Product schema represents the data of all the products in the platform. 
• It is used to store information about the product details, which will later be useful for ordering. 

c)	Orders Schema: <br>
• Schema: orders Schema 
• Model: ‘Orders’ 
• The Orders schema represents the orders data and includes fields such as userId, product Id, product name, quantity, size, order date, etc., 

d)	 Cart Schema: <br>
• Schema: cart Schema 
• Model: ‘Cart’ 
• The Cart schema represents the cart data and includes fields such as userId, product Id, product name, quantity, size, order date, etc., 
• The user Id field is a reference to the user who has the product in cart. 

e)	 Admin Schema:<br> 
• Schema: admin Schema 
• Model: ‘Admin’ 
• The admin schema has essential data such as categories, promoted restaurants, etc., 

f)	 Restaurant Schema:<br> 
• Schema: restaurant Schema 
• Model: ‘Restaurant’ 
• The restaurant schema has the info about the restaurant and it’s menu

<br>
4.	Setup Instructions<br>
•	Prerequisites: List of software dependencies<br>
a)	Node.js
b)	MongoDB and Mongoose
c)	Express.js
d)	React.js
e)	Git
f)	Visual Studio Code
<br>
Installation: Use Git for version control, enabling collaboration and tracking changes throughout the development process. Platforms like GitHub or Bitbucket can host your repository. 

• Git: Download and installation instructions can be found at: https://git scm.com/downloads 
Development Environment: Choose a code editor or Integrated Development Environment (IDE) that suits your preferences, such as Visual Studio Code, Sublime Text, or WebStorm.

 • Visual Studio Code: Download from https://code.visualstudio.com/download 

• Sublime Text: Download from https://www.sublimetext.com/download 

• WebStorm: Download from https://www.jetbrains.com/webstorm/download

To run the existing SB Foods App project downloaded from github:

a)	Clone the repository: <br>

• Open your terminal or command prompt. 
• Navigate to the directory where you want to store the required data. 

Install the required dependencies by running the following command: 
npm install 

b)	Start the Development Server: <br>

• To start the development server, execute the following command: 
   npm run dev or npm run start 
• The e-commerce app will be accessible at http://localhost:3000 by default. You can change the port configuration in the .env file if needed. 

c)	Access the App: <br>

• Open your web browser and navigate to http://localhost:3000. 
• You should see the food ordering homepage, indicating that the installation and setup were successful. .

5.	Folder Structure<br>
•	Client: The structure of the React frontend using VisualStudio code
 
<img width="219" height="591" alt="image" src="https://github.com/user-attachments/assets/2efe104a-0e31-4540-a803-28e6a20c7163" /><br>
📁 src/
Contains all the source code for the React app.<br>
✅ components/
      Reusable components used across multiple pages, such as:
Navbar.jsx
Footer.jsx
Login.jsx & Register.jsx – for authentication
Restaurants.jsx, PopularRestaurants.jsx – for listings<br>
✅ context/
Most likely for React Context API, where you manage global states such as user authentication, cart data, or selected restaurant.<br>
✅ images/
This would typically store all static image assets used in the UI.<br>
✅ pages/
All route-specific React pages are categorized into subfolders based on user type:
 ▶ admin/
Pages specifically for the admin dashboard:
AllUsers.jsx, AllProducts.jsx, AllRestaurants.jsx, AllOrders.jsx – for managing the platform
Admin.jsx – likely the main dashboard
▶ customer/
Pages for customers:
Cart.jsx – shows cart items
CategoryProducts.jsx – shows products by category
IndividualRestaurant.jsx – shows details of one restaurant
Profile.jsx – user profile
▶ restaurant/
Pages for restaurant owners:
NewProduct.jsx, EditProduct.jsx – manage their menu
RestaurantMenu.jsx, RestaurantOrders.jsx – view menu/orders
Authentication.jsx – possibly for login/register (restaurant-specific)
RestaurantHome.jsx – dashboard<br>
✅ Home.jsx
Likely the landing page of the application<br>
✅ styles/
Contains CSS or styling files (only App.css is shown).<br>
✅ App.js
Main entry point for routing and rendering pages.<br>

•	Server: <br>
1.	index.jsMain entry point for your backend server. Likely where you start the server, connect to MongoDB, and set up middleware and routes.
2.	Schema.jsDefines your MongoDB Mongoose schemas (data structure) — for example, Users, Products, Orders, Restaurants, etc.
3.	package.jsonLists your Node.js project's dependencies, scripts, name, and version.
4.	package-lock.jsonAuto-generated file that locks the versions of installed dependencies

6.	Running the Application:<br>
•	Provide commands to start the frontend and backend servers locally.
o	Frontend: npm start in the client directory.
o	Backend: npm start in the server directory.

7.	API Documentation<br>
•	Documentation of endpoints exposed by the backend.
All API endpoints are built using Express.js and communicate with the frontend using JSON.<br>
      Endpoints:
🔸 User Authentication<br>
POST /api/auth/register
Create a new user.
Body: { "username": "", "email": "", "password": "" }
POST /api/auth/login
Authenticate and return a token.
Body: { "email": "", "password": "" }
Response: { "token": "..." }
🔸 Products (Admin/Restaurant)<br>
GET /api/products
Returns all products.
POST /api/products
Adds a new product (admin/restaurant only).
🔸 Orders<br>
POST /api/orders
Places an order for the current user.
Body: { "userId": "", "items": [...], "total": 123 }
GET /api/orders/:userId
Get all orders for a user.
<br>
•	Including request methods, parameters, and example responses.
🔹 1. Register a New User<br>

Method: POST

Endpoint: /api/auth/register
Description: Registers a new user (customer or restaurant)
Request Body:<br>

{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "mypassword",
  "role": "customer"
}

Response:

{
  "message": "User registered successfully",
  "userId": "64d4fe9a01b12e..."
}

🔹 2. Login<br>
 Method: POST
Endpoint: /api/auth/login
Request Body:

{
  "email": "john@example.com",
  "password": "mypassword"
}

Response:

{
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6...",
  "user": {
    "id": "64d4fe9a01b12e...",
    "name": "John Doe",
    "role": "customer"
  }
}<br>
🔹 3. Get User Profile<br>
Method: GET
Endpoint: /api/auth/profile
Headers: Requires Authorization: Bearer <token>
Response:

{
  "id": "64d4fe9a01b12e...",
  "name": "John Doe",
  "email": "john@example.com",
  "role": "customer"
}<br>

🔹 4. Get All Products<br>
Method: GET
Endpoint: /api/products
Response:

[
  {
    "_id": "64d5acb99...",
    "name": "Pizza",
    "price": 250,
    "category": "Italian"
  }
]
<br>
8.	Authentication
• Create routes and middleware for user registration, login, and logout.
• Set up authentication middleware to protect routes that require user           authentication

9.	User Interface<br>
•	Provide screenshots or GIFs showcasing different UI features.
<img width="916" height="485" alt="image" src="https://github.com/user-attachments/assets/b06cdb2e-bfda-4772-bf33-dfe4869e9e8d" />
10.	Testing<br>
•	Describing the testing strategy and tools used.
Run tests using: npm test
Manual testing was conducted using the tools like:
Postman (for API testing)
Browser (React pages)

Form validations for login/register
Test Strategy: All major flows like user registration, login, cart functionality, and order placement were tested. 
<br>
11.	Screenshots or Demo<br>
•	Providing screenshots or a link to a demo to showcase the application.
	https://drive.google.com/file/d/1PImuicEGJGk4OnLiUU79Oh76MFuOHZqL/view?usp=drivesdk

12.	Known Issues<br>
 1. 🔑 No Password Reset
Users cannot reset their password in case they forget it. No recovery or email OTP mechanism is available.<br>
2. 📧 No Email Verification
Users can register with any email address without verification, which may lead to spam or fake accounts.<br>
3. 🔐 Token Storage Vulnerability
JWT tokens are stored in local Storage, which is vulnerable to cross-site scripting (XSS) attacks. Http Only cookies would be a more secure option.<br>
4. 📦 No Inventory or Stock Management
Products can be ordered repeatedly with no stock limit or quantity tracking.<br>
5. 💳 No Payment Gateway Integration
The application currently allows order placement but does not support online payment (e.g., Razorpay, Stripe).<br>

13.	Future Enhancements

The following features and improvements can be considered to enhance the functionality, security, and user experience of the OrderOnTheGo platform:

🌐 1. Payment Gateway Integration

Integrate Razorpay, Stripe, or PayPal for secure online payments.<br>

🔁 2. Real-time Order Status Tracking

Enable dynamic status updates for orders using technologies like WebSockets or Firebase.<br>

📧 3. Email/OTP Verification
Send mail confirmations and OTPs during registration or password recovery to verify user identity.<br>

🔑 4. Forgot Password & Password Reset

Add functionality for users to securely reset their password via email link or mobile OTP.<br>

📱 5. Progressive Web App (PWA) Support

Convert the app into a PWA so users can install it like a mobile app with offline support. 








