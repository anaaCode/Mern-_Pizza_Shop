# MERN Stack E-Pizza_Shop with Stripe Integration

## Project Description

This project is a comprehensive e-commerce platform developed using the MERN stack (MongoDB, Express.js, React.js, and Node.js). It aims to provide a robust foundation for building online stores with a seamless user experience and secure payment processing. The platform includes comprehensive product management, user authentication, order handling, and payment processing using the Stripe payment gateway.

## Features

### User Authentication and Authorization
- **Secure User Registration and Login**: Utilizes JWT (JSON Web Tokens) to ensure secure user authentication.
- **Role-Based Access Control**: Differentiates between customers and administrators to control access levels.

### Product Management
- **Admin Interface**: Allows administrators to add, edit, and delete products.
- **Product Listings**: Displays detailed descriptions, images, and pricing.
- **Search and Filter Functionality**: Enables users to easily find products.

### Shopping Cart
- **Cart Management**: Users can add, remove, and update product quantities in their cart.
- **Session Persistence**: Utilizes local storage to persist shopping cart data across sessions.

### Order Management
- **Order Placement**: Users can place orders with a summary of items, total price, and shipping details.
- **Admin Order Management**: Admins can manage and track orders, and update order statuses.

### Payment Processing
- **Stripe Integration**: Ensures secure payment handling through Stripe.
- **Multiple Payment Methods**: Supports various payment methods, including credit/debit cards.
- **Real-Time Payment Validation and Error Handling**: Provides immediate feedback on payment status.

### Responsive Design
- **Mobile-First Design**: Ensures a seamless user experience across all devices.
- **Intuitive User Interface**: Utilizes React components and Redux for state management.

## Technology Stack

### Frontend
- **React.js**: Utilized for building a dynamic and responsive user interface with reusable components.
- **Redux**: Manages the state across the application.
- **Bootstrap**: Provides responsive design and pre-styled components for a consistent look and feel.

### Backend
- **Node.js**: Runs the server-side application.
- **Express.js**: Builds RESTful APIs to handle CRUD operations and business logic.

### Database
- **MongoDB**: NoSQL database for storing user information, product details, orders, and other relevant data.
- **Mongoose**: ODM library to interact with MongoDB.

### Payment Gateway
- **Stripe**: Handles secure payment processing with Stripe API integration for transactions.

### Other Technologies
- **JWT**: Provides secure authentication and maintains user sessions.
- **Axios**: Facilitates HTTP requests from the client to the server.
- **Cloudinary**: Manages and hosts images for products.

## Project Structure

```
/Pizza_Shop
│
├── /backend
│   ├── /config
│   │   └── db.js          // Database connection setup
│   ├── /controllers
│   │   └── authController.js
│   │   └── productController.js
│   │   └── orderController.js
│   ├── /models
│   │   └── User.js
│   │   └── Product.js
│   │   └── Order.js
│   ├── /routes
│   │   └── authRoutes.js
│   │   └── productRoutes.js
│   │   └── orderRoutes.js
│   ├── server.js          // Main server file
│   └── .env               // Environment variables
│
├── /frontend
│   ├── /public
│   │   └── index.html     // HTML template
│   ├── /src
│   │   ├── /components
│   │   │   └── Header.js
│   │   │   └── Footer.js
│   │   │   └── ProductList.js
│   │   │   └── ProductDetail.js
│   │   ├── /pages
│   │   │   └── HomePage.js
│   │   │   └── ProductPage.js
│   │   │   └── CartPage.js
│   │   │   └── CheckoutPage.js
│   │   ├── /redux
│   │   │   └── store.js   // Redux store
│   │   │   └── reducers.js
│   │   │   └── actions.js
│   │   ├── App.js         // Main React component
│   │   ├── index.js       // Entry point for React
│   └── .env               // Environment variables
│
└── README.md              // Project documentation
```

## Installation and Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/anaaCode/Mern-_Pizza_Shop.git
   ```

2. **Backend Setup**:
   - Navigate to the backend directory:
     ```bash
     cd server
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Configure environment variables in `.env` file:
     ```
     MONGO_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     STRIPE_SECRET_KEY=your_stripe_secret_key
     CLOUDINARY_CLOUD_NAME=your_cloudinary_name
     CLOUDINARY_API_KEY=your_cloudinary_api_key
     CLOUDINARY_API_SECRET=your_cloudinary_api_secret
     ```
   - Start the backend server:
     ```bash
     npm start
     ```

3. **Frontend Setup**:
   - Navigate to the frontend directory:
     ```bash
     cd ../client
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the frontend development server:
     ```bash
     npm start
     ```

4. **Access the application**:
   - Open your browser and navigate to `http://localhost:3000` to view the application.

## Usage

- **User Registration and Login**: Users can register and log in to access their accounts.
- **Browse Products**: Users can browse, search, and filter products.
- **Shopping Cart**: Users can add products to their cart, update quantities, and remove items.
- **Checkout**: Users can proceed to checkout, enter shipping details, and make payments via Stripe.
- **Admin Panel**: Admins can manage products and orders through a dedicated interface.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for review.

## License

This project is licensed under the MIT License.

---

This project serves as a solid foundation for developing scalable and secure e-commerce applications using modern web technologies. By leveraging the power of the MERN stack and integrating with Stripe, it ensures a smooth and secure shopping experience for users.
