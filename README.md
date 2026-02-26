# 🚀 FlexiRent – Hybrid Rent & Buy Marketplace

A production-ready full-stack web application for renting and buying products with real product images, realistic pricing, and professional payment integration.

## ✨ Features

- 🛒 **Hybrid Marketplace** - Rent or Buy mode for each product
- 📸 **Real Product Images** - High-quality images with gallery & zoom
- 💳 **Payment Integration** - Razorpay with webhook verification
- 👥 **Multi-role System** - Users, Sellers, Admin
- 📅 **Advanced Rental Logic** - Date validation, inventory locking, late fees
- 🔐 **Secure Authentication** - JWT + Google OAuth
- 📊 **Analytics Dashboard** - Revenue, sales, bookings tracking
- 📱 **Fully Responsive** - Mobile, Tablet, Desktop optimized
- 🌙 **Dark/Light Mode** - Theme toggle included

## 🏗️ Tech Stack

### Frontend
- **Next.js 14** (App Router)
- **TypeScript**
- **Tailwind CSS**
- **Shadcn/ui** (Component library)
- **Zustand** (State management)

### Backend
- **Node.js**
- **Express.js**
- **MongoDB + Mongoose**
- **JWT Authentication**
- **Razorpay API**

### Deployment
- **Frontend** → Vercel
- **Backend** → Render

## 📁 Project Structure

```
FlexiRent/
├── frontend/          # Next.js application
│   ├── app/          # App router pages
│   ├── components/   # Reusable components
│   ├── hooks/        # Custom React hooks
│   ├── services/     # API services
│   ├── context/      # Context providers
│   ├── utils/        # Utility functions
│   └── tailwind.config.ts
├── backend/          # Express.js API
│   ├── routes/       # API endpoints
│   ├── controllers/  # Route handlers
│   ├── models/       # MongoDB schemas
│   ├── middleware/   # Custom middleware
│   ├── services/     # Business logic
│   ├── utils/        # Helper functions
│   └── config/       # Configuration
├── package.json
└── README.md
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- MongoDB (local or Atlas)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/prasath1108/FlexiRent.git
cd FlexiRent
```

2. **Install dependencies**
```bash
npm install
cd frontend && npm install
cd ../backend && npm install
cd ..
```

3. **Setup Environment Variables**

Create `.env.local` in `frontend/`:
```
NEXT_PUBLIC_API_URL=http://localhost:5000
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_google_client_id
```

Create `.env` in `backend/`:
```
MONGODB_URI=mongodb+srv://user:password@cluster.mongodb.net/flexirent
JWT_SECRET=your_jwt_secret
RAZORPAY_KEY_ID=your_razorpay_key
RAZORPAY_KEY_SECRET=your_razorpay_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

4. **Run Development Servers**
```bash
npm run dev
```

This will start both frontend (http://localhost:3000) and backend (http://localhost:5000) simultaneously.

## 📱 Pages Overview

### Public Pages
- **Home** - Featured products, categories, hero section
- **Products** - Advanced filtering, search, pagination
- **Product Detail** - Gallery, specs, reviews, rent/buy options
- **Cart** - Rental & purchase management
- **Checkout** - Payment processing

### User Dashboard
- **My Rentals** - Active & past rentals
- **My Purchases** - Order history
- **Wishlist** - Saved products
- **Profile** - Account management

### Seller Dashboard
- **My Products** - Add/edit products
- **Inventory** - Stock management
- **Earnings** - Revenue tracking
- **Analytics** - Sales reports

### Admin Panel
- **Users** - Manage user accounts
- **Sellers** - Approve/manage sellers
- **Products** - Content moderation
- **Disputes** - Handle claims
- **Analytics** - Platform metrics

## 🛍️ Featured Products

Real products with multiple images:
- 📷 Canon EOS 1500D DSLR Camera
- 💻 Gaming Laptop (RTX 4060)
- 🚲 Mountain Bike (29-inch)
- 🎮 PlayStation 5 Console
- 🎯 4K Office Projector
- ⌚ Apple Ultra Smartwatch
- 🚁 Professional Drone (4K)
- 🎪 Gaming Chair (RGB)
- 🔊 Bluetooth Speaker (360°)

## 💳 Payment Flow

### Rent Mode
1. Select dates
2. Add to cart (rental fee + security deposit)
3. Proceed to checkout
4. Razorpay payment
5. Order confirmation
6. Return & refund process

### Buy Mode
1. Select quantity
2. Add to cart
3. Proceed to checkout
4. Razorpay payment
5. Order confirmation
6. Shipping tracking

## 🔐 Authentication

- Email/Password signup
- Google OAuth login
- JWT-based sessions
- Role-based access control
- Secure password hashing

## 📊 Database Schema

### Collections
- **Users** - User accounts with roles
- **Products** - Product catalog
- **Rentals** - Rental transactions
- **Orders** - Purchase orders
- **Cart** - Shopping carts
- **Reviews** - Product reviews
- **Sellers** - Seller profiles
- **Disputes** - Damage/dispute claims

## 🎨 Design Features

- Soft shadows & rounded corners
- Smooth hover effects
- Skeleton loaders
- Toast notifications
- Responsive grid layouts
- Clean typography
- Professional color scheme
- Accessibility optimized

## 📦 Deployment

### Frontend (Vercel)
```bash
vercel deploy
```

### Backend (Render)
1. Push to GitHub
2. Connect Render to repository
3. Set environment variables
4. Deploy

## 📝 API Documentation

Full API documentation available at `/api/docs` after backend starts.

### Key Endpoints
- `POST /api/auth/signup` - User registration
- `POST /api/auth/login` - User login
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product details
- `POST /api/cart/add` - Add to cart
- `POST /api/payment/order` - Create payment order
- `POST /api/payment/verify` - Verify payment

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

MIT License - see LICENSE file for details

## 👨‍💻 Author

**Prasath** - [@prasath1108](https://github.com/prasath1108)

---

**⭐ If you find this useful, please star the repository!**