# Food Delivery App

A full-stack food delivery application built with React (Vite) for the frontend and admin panel, and Node.js/Express for the backend. This app allows users to browse food items, place orders, manage carts, and includes an admin panel for managing food listings and orders.

## Features

### Frontend (Customer App)
- Browse food items by category
- Add/remove items to/from cart
- User authentication (login/signup)
- Place orders and view order history
- Responsive design for mobile and desktop

### Admin Panel
- Add, edit, and delete food items
- View and manage orders
- Upload food images
- Dashboard for overview

### Backend
- RESTful API for food, users, orders, and cart management
- JWT-based authentication
- Image upload handling
- MongoDB for data storage

## Tech Stack

- **Frontend & Admin:** React, Vite, CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JWT
- **Image Handling:** Multer
- **Other:** Axios for API calls

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- Git

### Clone the Repository
```bash
git clone https://github.com/prince62058/food-delivery-app.git
cd food-delivery-app
```

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables: Create a `.env` file in the backend directory with the following:
   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=4000
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

### Admin Panel Setup
1. Navigate to the admin directory:
   ```bash
   cd ../admin
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Usage

- Access the frontend at `http://localhost:5173` (default Vite port)
- Access the admin panel at `http://localhost:5174` (default Vite port)
- Backend API runs on `http://localhost:4000`

### API Endpoints

#### Food
- `GET /api/food/list` - Get all food items
- `POST /api/food/add` - Add a new food item (admin)
- `POST /api/food/remove` - Remove a food item (admin)

#### User
- `POST /api/user/register` - Register a new user
- `POST /api/user/login` - Login user
- `GET /api/user/profile` - Get user profile

#### Cart
- `POST /api/cart/add` - Add item to cart
- `POST /api/cart/remove` - Remove item from cart
- `GET /api/cart/get` - Get cart items

#### Orders
- `POST /api/order/place` - Place an order
- `GET /api/order/userorders` - Get user orders
- `GET /api/order/list` - Get all orders (admin)
- `POST /api/order/status` - Update order status (admin)

## Project Structure

```
food-delivery-app/
├── admin/          # Admin panel (React/Vite)
├── backend/        # Backend API (Node.js/Express)
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── uploads/    # Uploaded images
├── frontend/       # Customer app (React/Vite)
└── README.md
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, feel free to open an issue on GitHub.
