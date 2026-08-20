# FoodRunner 🍔

Order food from local food vendors with ease. FoodRunner is a platform that connects food lovers with local vendors, enabling seamless ordering and delivery.

## Features

- 🔐 **User Authentication** - Secure login and registration
- 🍽️ **Vendor Profiles** - Browse local food vendors and their menus
- 🛒 **Shopping Cart** - Add items to cart and manage orders
- 💳 **Payment Integration** - Secure payment processing
- 📍 **Delivery Tracking** - Real-time order and delivery tracking
- ⭐ **Ratings & Reviews** - Rate vendors and leave reviews
- 🔔 **Notifications** - Get updates on your orders

## Tech Stack

### Frontend
- React 18+
- Redux for state management
- Tailwind CSS for styling
- React Router for navigation
- Axios for API calls

### Backend
- Node.js with Express
- MongoDB for database
- JWT for authentication
- Stripe/Razorpay for payments
- Socket.io for real-time updates

## Project Structure

```
FoodRunner/
├── frontend/                 # React application
│   ├── public/
│   ├── src/
│   │   ├── components/      # Reusable components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API services
│   │   ├── store/           # Redux store
│   │   └── App.js
│   └── package.json
├── backend/                  # Express server
│   ├── models/              # Database models
│   ├── routes/              # API routes
│   ├── controllers/         # Request handlers
│   ├── middleware/          # Custom middleware
│   ├── config/              # Configuration files
│   ├── server.js
│   └── package.json
├── docs/                    # Documentation
└── .gitignore
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/emmanuelshedrach21-lab/FoodRunner.git
   cd FoodRunner
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   cp .env.example .env
   # Configure your .env file with database and payment credentials
   npm run dev
   ```

3. **Setup Frontend**
   ```bash
   cd ../frontend
   npm install
   cp .env.example .env
   # Configure your .env file with API URL
   npm start
   ```

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Vendors
- `GET /api/vendors` - Get all vendors
- `GET /api/vendors/:id` - Get vendor details
- `GET /api/vendors/:id/menu` - Get vendor menu

### Orders
- `POST /api/orders` - Create order
- `GET /api/orders/:id` - Get order details
- `GET /api/orders` - Get user orders
- `PUT /api/orders/:id` - Update order status

### Reviews
- `POST /api/reviews` - Create review
- `GET /api/vendors/:id/reviews` - Get vendor reviews

## Contributing

1. Create a feature branch (`git checkout -b feature/AmazingFeature`)
2. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
3. Push to the branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, email support@foodrunner.com or open an issue in the repository.

---

**Happy coding! 🚀**
