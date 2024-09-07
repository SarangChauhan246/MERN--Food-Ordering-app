

# MERN Food Ordering App

## Project Overview
The **MERN Food Ordering App** is a web-based application designed to streamline the process of ordering food from various restaurants. This app enables users to browse menus, select items, place orders, and make payments online. It also includes authentication features using Auth0, and provides an admin interface for managing orders, users, and menu items.

## Features
- **User Authentication:** Secure login and registration using Auth0.
- **Browse Menu:** Users can browse through the available menu items from different restaurants.
- **Order Food:** Users can add items to the cart, review the order, and place an order.
- **Payment Integration:** Online payment functionality for order completion.
- **Admin Interface:** Admins can manage menu items, view orders, and handle user accounts.
- **Responsive Design:** Fully responsive design, optimized for both desktop and mobile devices.

## Tech Stack
- **Frontend:**
  - React.js
  - Redux (for state management)
  - Tailwind CSS (for styling)
  - Axios (for API calls)
- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (Mongoose for ORM)
- **Authentication:**
  - Auth0
- **Deployment:**
  - MongoDB Atlas (for database hosting)
  - Vercel/Netlify (for frontend hosting)
  - Heroku/AWS EC2 (for backend hosting)

## Installation

### Prerequisites
Ensure you have the following installed on your local machine:
- Node.js
- npm or yarn
- MongoDB (local or MongoDB Atlas for cloud-based database)

### Backend Setup
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd mern-food-ordering-app
   ```

2. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

4. Set up environment variables by creating a `.env` file in the `backend` directory:
   ```bash
   touch .env
   ```

   Add the following environment variables:
   ```env
   MONGO_URI=<your-mongodb-uri>
   PORT=5000
   VITE_API_BASE_URL=http://localhost:5000
   AUTH0_DOMAIN=<your-auth0-domain>
   AUTH0_CLIENT_ID=<your-auth0-client-id>
   AUTH0_CALLBACK_URL=http://localhost:3000
   ```

5. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the `frontend` directory:
   ```bash
   touch .env
   ```

   Add the following environment variables:
   ```env
   VITE_API_BASE_URL=http://localhost:5000
   VITE_AUTH0_DOMAIN=<your-auth0-domain>
   VITE_AUTH0_CLIENT_ID=<your-auth0-client-id>
   VITE_AUTH0_CALLBACK_URL=http://localhost:3000
   ```

4. Start the frontend development server:
   ```bash
   npm start
   ```

## Usage
1. Visit the frontend URL (typically `http://localhost:3000`).
2. Register or log in using Auth0.
3. Browse the menu, add items to the cart, and place an order.
4. Admin users can log in and access the admin dashboard to manage orders and menu items.

## Deployment
- **Frontend:** Deploy to Vercel or Netlify.
- **Backend:** Deploy to Heroku, AWS EC2, or any Node.js hosting provider.
- **Database:** Use MongoDB Atlas for cloud-based MongoDB hosting.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License
This project is licensed under the MIT License.


