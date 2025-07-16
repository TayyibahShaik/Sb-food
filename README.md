DEMO-
<a href="https://drive.google.com/file/d/1RJzLnoh63AlDz6dUwKgoZcZq9fA9gZwX/view?usp=drive_link">Demo Video </a>

<hr>
<b> </b>FOOD ORDERING APPLICATION </b>
<b>INTRODUCTION</b>

•	 Project Title: OrderOnTheGo: Your On-Demand Food Ordering Solution 
•	Team Members: Shaik Tayyibah, C Sunitha, V Anitha, V Sherylinpaul.
•	Roles in Project:  Project Setup and Configuration & Frontend development were done by C Sunitha and V Sherylinpaul
 Backend Development, Database Development & Project Implementation and Execution were done by Shaik Tayyibah and V Anitha


Introducing SB Foods, the cutting-edge digital platform poised to revolutionize the way you order food online. With SB Foods, your food ordering experience will reach unparalleled levels of convenience and efficiency.
Our user-friendly web app empowers foodies to effortlessly explore, discover, and order dishes tailored to their unique tastes. Whether you're a seasoned food enthusiast or an occasional diner, finding the perfect meals has never been more straightforward.
Imagine having comprehensive details about each dish at your fingertips. From dish descriptions and customer reviews to pricing and available promotions, you'll have all the information you need to make well-informed choices. No more second-guessing or uncertainty – SB Foods ensures that every aspect of your online food ordering journey is crystal clear.
The ordering process is a breeze. Just provide your name, delivery address, and preferred payment method, along with your desired dishes. Once you place your order, you'll receive an instant confirmation. No more waiting in long queues or dealing with complicated ordering processes – SB Foods streamlines it, making it quick and hassle-free.

SCENARIO: 
Late-Night Craving Resolution
Meet Lisa, a college student burning the midnight oil to finish her assignment. As the clock strikes midnight, her stomach grumbles, reminding her that she skipped dinner. Lisa doesn't want to interrupt her workflow by cooking, nor does she have the energy to venture outside in search of food.
Solution with Food Ordering App:
1. Lisa opens the Food Ordering App on her smartphone and navigates to the late-night delivery section, where she finds a variety of eateries still open for orders.
2. She scrolls through the options, browsing menus and checking reviews until she spots her favorite local diner offering comfort food classics.
3. Lisa selects a hearty bowl of chicken noodle soup and a side of garlic bread, craving warmth and satisfaction in each bite.
4. With a few taps, she adds the items to her cart, specifies her delivery address, and chooses her preferred payment method.
5. Lisa double-checks her order details on the confirmation page, ensuring everything looks correct, before tapping the "Place Order" button.
6. Within minutes, she receives a notification confirming her order and estimated delivery time, allowing her to continue working with peace of mind.
7. As promised, the delivery arrives promptly at her doorstep, and Lisa eagerly digs into her piping hot meal, grateful for the convenience and comfort provided by the Food Ordering App during her late-night study session.

This scenario illustrates how a Food Ordering App caters to users' needs, even during unconventional hours, by offering a seamless and convenient solution for satisfying late-night cravings without compromising on quality or convenience.


<b>TECHNICAL ARCHITECTURE: </b>
 
In this architecture diagram:
•        The frontend is represented by the "Frontend" section, including user interface components such as User Authentication, Cart, Products, Profile, Admin dashboard, etc.,
•        The backend is represented by the "Backend" section, consisting of API endpoints for Users, Orders, Products, etc., It also includes Admin Authentication and an Admin Dashboard.
•        The Database section represents the database that stores collections for Users, Admin, Cart, Orders, and products.
<b>FEATURES:</b> 
1. Comprehensive Product Catalog: SB Foods boasts an extensive catalog of food items from  various restaurants, offering a diverse range of items and options for shoppers. You can  effortlessly explore and discover various products, complete with detailed descriptions,  customer reviews, pricing, and available discounts, to find the perfect food for your hunger. 
2. Order Details Page: Upon clicking the "Shop Now" button, you will be directed to an order  details page. Here, you can provide relevant information such as your shipping address,  preferred payment method, and any specific product requirements. 
3. Secure and Efficient Checkout Process: SB Foods guarantees a secure and efficient checkout  process. Your personal information will be handled with the utmost security, and we strive to  make the purchasing process as swift and trouble-free as possible. 
4. Order Confirmation and Details: After successfully placing an order, you will receive a  confirmation notification. Subsequently, you will be directed to an order details page, where  you can review all pertinent information about your order, including shipping details, payment  method, and any specific product requests you specified. 
In addition to these user-centric features, SB Foods provides a robust restaurant dashboard,  offering restaurants an array of functionalities to efficiently manage their products and sales.  With the restaurant dashboard, restaurants can add and oversee multiple product listings, view  order history, monitor customer activity, and access order details for all purchases. 
SB Foods is designed to elevate your online food ordering experience by providing a seamless  and user-friendly way to discover your desired foods. With our efficient checkout process,  comprehensive product catalog, and robust restaurant dashboard, we ensure a convenient and  enjoyable online shopping experience for both shoppers and restaurants alike.<br>
<b>FRONTEND DEVELOPMENT: </b>
1. Setup React Application: 
• Create a React app in the client folder. 
• Install required libraries 
• Create required pages and components and add routes. 
2.Design UI components: 
• Create Components. 
• Implement layout and styling. 
• Add navigation. 
3.Implement frontend logic: 
• Integration with API endpoints. 
• Implement data binding. 
Demo UI images:
·       Landing page
<img width="1023" height="542" alt="image" src="https://github.com/user-attachments/assets/1f79da85-66e1-4ed9-9a10-54819ae0b62d" />
Restaurant : 
• Schema: restaurantSchema 
• Model: ‘Restaurant’ 
• The restaurant schema has the info about the restaurant and it’s menu
<img width="1023" height="544" alt="image" src="https://github.com/user-attachments/assets/c3c0af84-f4ac-4fab-a26c-3930cd39ef01" />
<img width="1023" height="540" alt="image" src="https://github.com/user-attachments/assets/5bdc9392-46fe-41da-94e3-b9b95bd09d09" />
Cart: 
• Schema: cartSchema 
• Model: ‘Cart’ 
• The Cart schema represents the cart data and includes fields such as userId, product  Id, product name, quantity, size, order date, etc., 
• The user Id field is a reference to the user who has the product in cart.
<img width="1023" height="531" alt="image" src="https://github.com/user-attachments/assets/0d0f9311-dbf7-4a59-9967-8b161d38df04" />
<img width="1023" height="527" alt="image" src="https://github.com/user-attachments/assets/5ad0b2a8-02a2-4b47-856c-8ef00bc7f42c" />

Admin : 
• Schema: adminSchema 
• Model: ‘Admin’ 
• The admin schema has essential data such as categories, promoted restaurants, etc., 
<img width="1023" height="538" alt="image" src="https://github.com/user-attachments/assets/ecbd7816-c206-4de3-9a6c-2e888bc33ba3" />
<img width="1023" height="531" alt="image" src="https://github.com/user-attachments/assets/870b60a7-bde1-4ec8-b8b1-5fa8aab3afc8" />
<b>BACKEND DEVELOPMENT: </b>
1. Setup express server: 
• Create index.js file. 
• Create an express server on your desired port number.
• Define API’s
2. Database Configuration: 
• Set up a MongoDB database either locally or using a cloud-based MongoDB service like MongoDB Atlas or use locally with MongoDB compass. 
• Create a database and define the necessary collections for admin, users,  restaurants, food products, orders,and other relevant data. 

Create Express.js Server: 
• Set up an Express.js server to handle HTTP requests and serve API endpoints.
 • Configure middleware such as body-parser for parsing request bodies and cors for handling cross-origin requests.
4. Define API Routes: 
• Create separate route files for different API functionalities such as users, orders, and authentication. 
• Define the necessary routes for listing products, handling user registration and  login,managing orders, etc. 
• Implement route handlers using Express.js to handle requests and interact with the database. 
5. Implement Data Models: 
• Define Mongoose schemas for the different data entities like products, users,  and orders. 
• Create corresponding Mongoose models to interact with the MongoDB database.
 • Implement CRUD operations (Create, Read, Update, Delete) for each model to perform database operations. 
6. User Authentication: 
• Create routes and middleware for user registration, login, and logout. 
• Set up authentication middleware to protect routes that require user authentication. 
<img width="1023" height="535" alt="image" src="https://github.com/user-attachments/assets/6a6b5541-9614-46ca-ad98-4ad20f49e2b7" />

7. Handle new products and Orders: 
• Create routes and controllers to handle new product listings, including fetching products data from the database and sending it as a response. 
• Implement ordering(buy) functionality by creating routes and controllers to  handle order requests, including validation and database updates. 

For any further doubts or help, please consider the GitHub repo, 
https://github.com/TayyibahShaik/Sb-food








